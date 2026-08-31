# Receipts Ledger — Weekly Digest

_Last updated: 2026-08-31_

## New charges this run
Searched `label:Receipts newer_than:8d` (5 threads found, all new - deduped
against every `message_id` already in the ledger). **5 rows appended:**

- **Canva Pro** — invoice 04987-68600509, **$15.90**, 2026-08-28. Same as
  prior months - no price change.
- **Anthropic (Claude Pro)** — **new vendor**. Receipt #2927-5998-6603,
  **$21.40** ($20.00 + $1.40 WV tax), 2026-08-26, billing period Aug
  26-Sep 26. Addressed to the dotless variant of Deb's Gmail address
  (Gmail ignores dots, so it's the same mailbox) - not a red flag, just
  worth noting.
- **Pool Pals, LLC** — three more overdue reminders for invoice #1511
  (2026-08-26, 2026-08-27, 2026-08-28). No new invoice this run.

## Current confirmed monthly recurring total: **$230.98/mo**
Unchanged from last week: PriceLabs $39.20 + Canva Pro $15.90 + Breezeway
$49.98 + Xfinity ...4222 $55.00 + Xfinity ...6337 $70.90.

## 🚩 Flags

- **New vendor: Anthropic (Claude Pro), $21.40/mo.** First-ever charge
  under this label. Confirm this subscription is intentional - if so,
  it'll add ~$21.40/mo to the confirmed total once a second month
  confirms the price.
- **Pool Pals invoice #1511 slow-pay pattern intensifying.** That single
  invoice (opened 2026-08-18) has now drawn **5** overdue reminders
  (08-19, 08-20, 08-26, 08-27, 08-28) with no new invoice in between.
  Worth confirming it's actually been paid - this may just be Pool Pals'
  reminder system not updating.

No price changes, no duplicate subscriptions or charges, and no charges
tied to a paused project this week (paused list is still empty - see
`ledger/paused_projects.json`).

Carried over from prior weeks, still worth a look if not already resolved:
- **Potomac Edison** (both properties) - new vendor flagged 2026-08-10,
  still only one statement each so far ($158.74 1030 Shannondale +
  $202.36 704 Valley View). Needs a second month's statement to confirm
  the recurring pattern.
- **QR Code Generator Pro** ($119.88, 2026-08-05) - new vendor, likely an
  annual plan. Confirm this was intentional.
- **PriceLabs** price change ($37.08 → $39.20, +5.7%) from 2026-06-15,
  confirmed steady through 2026-08-03.
- **Apple Valley Waste** two consecutive price increases ($228.58 →
  $241.00 → $253.90, ~+5.3-5.4% each) - worth confirming this is a
  published rate increase.

## Vendors tracked

| Vendor | Category | Billing cycle | Last known charge | Status |
|---|---|---|---|---|
| PriceLabs | Software subscription | Monthly | $39.20 · 2026-08-03 | active, price changed |
| Canva Pro | Software subscription | Monthly | $15.90 · 2026-08-28 | active, stable |
| Breezeway | Software subscription | Monthly | $49.98 · 2026-08-05 | active, stable |
| Xfinity (...4222) | Utility | Monthly | $55.00 · 2026-08-12 (bill notice, AutoPay 2026-09-03) | active, stable |
| Xfinity (...6337) | Utility | Monthly | $70.90 · 2026-08-22 (bill notice, AutoPay 2026-09-14) | active, stable |
| Apple Valley Waste | Utility | Quarterly | $253.90 · 2026-05-30 | active, price rising |
| QR Code Generator Pro | Software subscription | Unknown | $119.88 · 2026-08-05 | new, unconfirmed |
| Pool Pals, LLC | Service | Irregular | amount unknown · 2026-08-28 (5th reminder; invoice #1511 · 2026-08-18) | active, frequently overdue |
| Petti Pest Control | Service | Irregular | amount unknown · 2026-08-21 (invoice #341342; inspection report same day, 704 Valley View Rd) | active |
| Booking.com (host invoices) | Platform commission | Irregular | amount unknown · 2026-08-06 (last invoice) | active, 2 listings |
| Potomac Edison (...6615, 1030 Shannondale) | Utility | Monthly | $158.74 · 2026-08-07 (statement) | new, unconfirmed |
| Potomac Edison (...8822, 704 Valley View) | Utility | Monthly | $202.36 · 2026-08-06 (statement) | new, unconfirmed |
| Anthropic (Claude Pro) | Software subscription | Monthly | $21.40 · 2026-08-26 | new, unconfirmed |

Full history and machine-readable detail: `ledger/vendors.json`.
Paused-project list: `ledger/paused_projects.json`.
Process this file is generated from: `ledger/RUNBOOK.md`.
