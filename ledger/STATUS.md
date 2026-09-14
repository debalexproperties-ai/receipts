# Receipts Ledger — Weekly Digest

_Last updated: 2026-09-14_

## New charges this run
Searched `label:Receipts newer_than:8d` (3 threads / 3 messages found, all
new - deduped against every `message_id` already in the ledger). Rows
appended across 2 vendors:

- **Xfinity (...4222)** — $55.00 bill-available statement, 2026-09-12.
  AutoPay scheduled for 2026-10-03. Same as last month - no price change.
- **Pool Pals, LLC** — two more overdue reminders for invoice #1511
  (2026-09-08, 21 days overdue; 2026-09-09, 22 days overdue), bringing that
  single still-open invoice to **10** reminders since it opened 2026-08-18.
  Balance confirmed again at **$498.20**. Still no new invoice or payment
  confirmation.

## Current confirmed monthly recurring total: **$614.68/mo**
Unchanged from last week - no vendor's status, cycle, or price moved this
run: PriceLabs $39.20 + Canva Pro $15.90 + Breezeway $49.98 + Xfinity
...4222 $55.00 + Xfinity ...6337 $70.90 + Potomac Edison ...6615 $189.75 +
Potomac Edison ...8822 $193.95.

## 🚩 Flags

**No new-vendor, price-change, duplicate-subscription/charge, or
paused-project flags this week** (paused list is still empty - see
`ledger/paused_projects.json`). One thing worth your attention anyway:

- **Pool Pals invoice #1511 slow-pay streak continues.** Now **10**
  overdue reminders (08-19, 08-20, 08-26, 08-27, 08-28, 09-01, 09-02, 09-04,
  09-08, 09-09) spanning nearly 4 weeks with no new invoice in between, and
  the balance is still confirmed at **$498.20**. Recommend contacting Pool
  Pals directly to confirm whether this has actually been paid - their
  reminder system may just not be updating.

Carried over from prior weeks, still worth a look if not already resolved:
- **QR Code Generator Pro** ($119.88, 2026-08-05) - new vendor, likely an
  annual plan. Confirm this was intentional.
- **Anthropic (Claude Pro)** ($21.40/mo, first charge 2026-08-26) - only
  one data point so far; not yet in the confirmed monthly total.
- **PriceLabs** price change ($37.08 → $39.20, +5.7%) from 2026-06-15,
  confirmed steady through 2026-09-03.
- **Apple Valley Waste** two consecutive price increases ($228.58 →
  $241.00 → $253.90, ~+5.3-5.4% each) - worth confirming this is a
  published rate increase.

## Vendors tracked

| Vendor | Category | Billing cycle | Last known charge | Status |
|---|---|---|---|---|
| PriceLabs | Software subscription | Monthly | $39.20 · 2026-09-03 | active, stable |
| Canva Pro | Software subscription | Monthly | $15.90 · 2026-08-28 | active, stable |
| Breezeway | Software subscription | Monthly | $49.98 · 2026-09-03 | active, stable |
| Xfinity (...4222) | Utility | Monthly | $55.00 · 2026-09-12 (bill notice, AutoPay 2026-10-03) | active, stable |
| Xfinity (...6337) | Utility | Monthly | $70.90 · 2026-08-22 (bill notice, AutoPay 2026-09-14) | active, stable |
| Apple Valley Waste | Utility | Quarterly | $253.90 · 2026-05-30 | active, price rising |
| QR Code Generator Pro | Software subscription | Unknown | $119.88 · 2026-08-05 | new, unconfirmed |
| Pool Pals, LLC | Service | Irregular | $498.20 · 2026-09-09 (10th reminder; invoice #1511 · 2026-08-18) | active, frequently overdue |
| Petti Pest Control | Service | Irregular | amount unknown · 2026-09-03 (inspection report, 1030 Shannondale Rd) | active |
| Booking.com (host invoices) | Platform commission | Irregular | amount unknown · 2026-09-06 (last invoice) | active, 2 listings |
| Potomac Edison (...6615, 1030 Shannondale) | Utility | Monthly | $189.75 · 2026-09-04 (statement) | active, usage-based |
| Potomac Edison (...8822, 704 Valley View) | Utility | Monthly | $193.95 · 2026-09-04 (statement) | active, usage-based |
| Anthropic (Claude Pro) | Software subscription | Monthly | $21.40 · 2026-08-26 | new, unconfirmed |

Full history and machine-readable detail: `ledger/vendors.json`.
Paused-project list: `ledger/paused_projects.json`.
Process this file is generated from: `ledger/RUNBOOK.md`.
