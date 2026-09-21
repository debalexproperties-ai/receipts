# Receipts Ledger — Weekly Digest

_Last updated: 2026-09-21_

## New charges this run
Searched `label:Receipts newer_than:8d` (6 threads / 6 messages found, all
new - deduped against every `message_id` already in the ledger). Rows
appended across 3 vendors:

- **Xfinity (...6337)** — $70.90 payment confirmation, 2026-09-15. AutoPay
  processed successfully, completing the payment scheduled from the
  2026-08-22 statement. Same as last month - no price change.
- **Apple Valley Waste** — new invoice #0007157561, $251.10, 2026-09-16
  (account #310718). Down $2.80 (-1.1%) from the prior $253.90 invoice -
  a small dip after two consecutive ~5% increases, treated as normal
  variability rather than a price change.
- **Petti Pest Control** — one inspection report at 704 Valley View Rd
  (2026-09-14, no charge) and one invoice #352282 (2026-09-14, amount
  inside a PDF attachment and not extracted, per known limitation).
- **Pool Pals, LLC** — two more overdue reminders for invoice #1511
  (2026-09-14, 27 days overdue; 2026-09-16, 29 days overdue), bringing
  that single still-open invoice to **12** reminders since it opened
  2026-08-18. Balance confirmed again at **$498.20**. Still no new invoice
  or payment confirmation.

## Current confirmed monthly recurring total: **$614.68/mo**
Unchanged from last week - no monthly vendor's status, cycle, or price
moved this run: PriceLabs $39.20 + Canva Pro $15.90 + Breezeway $49.98 +
Xfinity ...4222 $55.00 + Xfinity ...6337 $70.90 + Potomac Edison ...6615
$189.75 + Potomac Edison ...8822 $193.95.

## 🚩 Flags

**No new-vendor, price-change, duplicate-subscription/charge, or
paused-project flags this week** (paused list is still empty - see
`ledger/paused_projects.json`). Two things worth your attention anyway:

- **Pool Pals invoice #1511 slow-pay streak continues, now over 5 weeks.**
  **12** overdue reminders (08-19, 08-20, 08-26, 08-27, 08-28, 09-01,
  09-02, 09-04, 09-08, 09-09, 09-14, 09-16) with no new invoice in between,
  balance still confirmed at **$498.20**. This has gone on long enough
  that it's worth contacting Pool Pals directly this week rather than
  waiting for another reminder - either it's been paid and their system
  isn't updating, or it genuinely needs to be settled.
- **Apple Valley Waste price dipped slightly** ($253.90 → $251.10, -1.1%)
  after two straight increases. Not flagged as a real price change, just
  noting the reversal.

Carried over from prior weeks, still worth a look if not already resolved:
- **QR Code Generator Pro** ($119.88, 2026-08-05) - new vendor, likely an
  annual plan. Confirm this was intentional.
- **Anthropic (Claude Pro)** ($21.40/mo, first charge 2026-08-26) - only
  one data point so far; not yet in the confirmed monthly total.
- **PriceLabs** price change ($37.08 → $39.20, +5.7%) from 2026-06-15,
  confirmed steady through 2026-09-03.

## Vendors tracked

| Vendor | Category | Billing cycle | Last known charge | Status |
|---|---|---|---|---|
| PriceLabs | Software subscription | Monthly | $39.20 · 2026-09-03 | active, stable |
| Canva Pro | Software subscription | Monthly | $15.90 · 2026-08-28 | active, stable |
| Breezeway | Software subscription | Monthly | $49.98 · 2026-09-03 | active, stable |
| Xfinity (...4222) | Utility | Monthly | $55.00 · 2026-09-12 (bill notice, AutoPay 2026-10-03) | active, stable |
| Xfinity (...6337) | Utility | Monthly | $70.90 · 2026-09-15 (payment confirmed) | active, stable |
| Apple Valley Waste | Utility | Quarterly | $251.10 · 2026-09-16 | active, price steady |
| QR Code Generator Pro | Software subscription | Unknown | $119.88 · 2026-08-05 | new, unconfirmed |
| Pool Pals, LLC | Service | Irregular | $498.20 · 2026-09-16 (12th reminder; invoice #1511 · 2026-08-18) | active, frequently overdue |
| Petti Pest Control | Service | Irregular | amount unknown · 2026-09-14 (invoice #352282) | active |
| Booking.com (host invoices) | Platform commission | Irregular | amount unknown · 2026-09-06 (last invoice) | active, 2 listings |
| Potomac Edison (...6615, 1030 Shannondale) | Utility | Monthly | $189.75 · 2026-09-04 (statement) | active, usage-based |
| Potomac Edison (...8822, 704 Valley View) | Utility | Monthly | $193.95 · 2026-09-04 (statement) | active, usage-based |
| Anthropic (Claude Pro) | Software subscription | Monthly | $21.40 · 2026-08-26 | new, unconfirmed |

Full history and machine-readable detail: `ledger/vendors.json`.
Paused-project list: `ledger/paused_projects.json`.
Process this file is generated from: `ledger/RUNBOOK.md`.
