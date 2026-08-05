# Weekly Receipts Ledger — Runbook

This repo maintains a running ledger of every vendor charge found under the
**Receipts** label in deb.alex.properties@gmail.com, and flags anomalies:
new vendors, price changes, duplicate subscriptions, and charges tied to
paused projects.

A scheduled Routine fires into a fresh session every **Monday ~7am ET**
and should follow this runbook exactly. If you're that session, start here.

## 1. Get to the right state

```
git fetch origin claude/gmail-receipts-ledger-s235of
git checkout claude/gmail-receipts-ledger-s235of || git checkout -b claude/gmail-receipts-ledger-s235of origin/claude/gmail-receipts-ledger-s235of
git pull
```

If the branch has since been merged into the default branch, treat this as
a fresh cycle: branch again from the default branch with the same name and
keep going.

Read `ledger/vendors.json` (the ledger) and `ledger/paused_projects.json`
(the paused list) before doing anything else.

## 2. Pull this week's receipts

Search Gmail:

```
label:Receipts newer_than:8d
```

The 8-day window (vs. the 7-day cadence) is deliberate overlap so a
slightly-late email never falls in a gap between runs. That overlap is
made safe by deduping: **before adding anything, check its Gmail message id
against every `message_id` already present in `ledger/vendors.json`.** If
it's already there, skip it - never add the same message twice.

For each remaining receipt, extract: **vendor, date, amount, and billing
cycle**. Most vendors put the amount right in the search-result snippet;
call `get_message` for the full body only when the snippet doesn't show one
(Canva, Breezeway, and QR Code Generator Pro have shown amounts in the HTML
body even when the preview snippet was blank).

**Known limitation:** Pool Pals, Petti Pest Control, and Booking.com host
invoices carry their dollar amount inside a PDF attachment or an external
portal - this Gmail MCP toolset has no attachment-download tool, so log the
occurrence (date, message id, type) with `amount: null` rather than
guessing.

## 3. Append and flag

Append the new, deduped rows to the vendor's `charges` array in
`ledger/vendors.json` (new vendor → add a new entry with `"status": "new"`).
Don't rewrite history - this file's job is to grow, and its git diff is the
audit trail.

Then check each of the following, in this order:

1. **New vendor** - sender/vendor not already in `vendors.json` → flag
   `new_vendor` on its first charge. The single most important check.
2. **Price change** - new charge amount differs from that vendor's most
   recent charge (same billing-cycle vendor, e.g. same Xfinity account) →
   flag `price_change` with old → new and % change. Ignore cents of tax
   rounding jitter; flag real plan-level moves.
3. **Possible duplicate subscription** - two active vendors whose
   `category` + `purpose` overlap (e.g. two dynamic-pricing tools, two
   design tools) → flag `duplicate_subscription`. This needs judgment:
   read every active vendor's `purpose` field, don't string-match blindly.
   Also check for a plain **duplicate charge**: the same vendor + same
   amount billed twice inside one normal billing cycle → flag
   `duplicate_charge`. Don't confuse this with known duplicate-*send*
   glitches already logged for Petti Pest Control (near-identical
   timestamps seconds apart = one event delivered twice, not two charges).
4. **Paused-project charge** - check the new vendor/charge against
   `ledger/paused_projects.json`. Any match → flag `paused_project_charge`.

## 4. Recompute the confirmed monthly recurring total

Recalculate `meta.confirmed_monthly_recurring_total` in `vendors.json`:
sum the **latest** charge amount for every vendor where `billing_cycle`
contains "monthly" and `status` is "active". Update `basis` to list which
vendors went into the sum (this changes whenever a vendor's cycle,
status, or price changes). Update `as_of` to today's date.

## 5. Update the status digest

Rewrite `ledger/STATUS.md` in full (don't hand-edit) as a short digest:
**new charges this week, current confirmed monthly recurring total
("monthly burn"), and flags** (new vendor / price change / duplicate
subscription or charge / paused-project charge - or "no flags this week").
Keep the per-vendor summary table below it for reference.

Update `meta.last_run` and `meta.last_message_date_processed` (the date of
the newest message processed this run).

## 6. Commit and push

```
git add ledger/
git commit -m "Weekly receipts ledger update: <one-line summary of flags>"
git push -u origin claude/gmail-receipts-ledger-s235of
```

Use retries with backoff on network failures, per standing git instructions.

## 7. Close out with the digest

End your final reply with the same short digest you wrote to
`ledger/STATUS.md`: **new charges, current monthly burn, flags** (or "no
flags this week"). This is what gets emailed to
deb.alex.properties@gmail.com, so it needs to read standalone.

## Notes for future refinement

- Xfinity account `...4222` and `...6337` are two separate properties;
  we haven't confirmed which physical address maps to which account
  number. Not needed for anomaly detection.
- If PDF-attachment amounts (Pool Pals, Petti Pest Control) become
  important enough to track precisely, the fix is adding an
  attachment-read capability, not trying harder with the current tools.
- Booking.com "booking confirmed" emails (Deb as guest, e.g. hotel stays)
  are personal travel and out of scope for this ledger - don't add them as
  vendors.
- `ledger/paused_projects.json` starts empty. Add an entry any time a
  vendor/property/subscription is intentionally put on hold, so future
  runs can catch a charge that shouldn't still be happening.
