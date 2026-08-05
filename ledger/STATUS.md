# Receipts Ledger — Weekly Digest

_Last updated: 2026-08-05_

## New charges this run
Searched `label:Receipts newer_than:8d` (5 threads found; **all 5 were
already in the ledger** from the prior run - same Gmail message ids,
deduped and skipped). No new rows appended this run.

## Current confirmed monthly recurring total: **$230.98/mo**
PriceLabs $39.20 + Canva Pro $15.90 + Breezeway $49.98 + Xfinity ...4222
$55.00 + Xfinity ...6337 $70.90. Unchanged from last run - no price moves
this week. Excludes QR Code Generator Pro (cycle unconfirmed), Apple Valley
Waste (quarterly), and Pool Pals / Petti Pest Control / Booking.com
(irregular, amount unknown).

## 🚩 Flags

**No flags this week** - no new vendors, no price changes, no duplicate
subscriptions or charges, and no charges tied to a paused project (the
paused list is still empty - see `ledger/paused_projects.json`).

Carried over from prior weeks, still worth a look if not already resolved:
- **QR Code Generator Pro** ($119.88, 2026-08-05) - new vendor flagged
  previously, likely an annual plan. Confirm this was intentional.
- **PriceLabs** price change ($37.08 → $39.20, +5.7%) from the 2026-06-15
  cycle, now confirmed steady through 2026-08-03.
- **Apple Valley Waste** two consecutive price increases ($228.58 →
  $241.00 → $253.90, ~+5.3-5.4% each) - worth confirming this is a
  published rate increase.

## Vendors tracked

| Vendor | Category | Billing cycle | Last known charge | Status |
|---|---|---|---|---|
| PriceLabs | Software subscription | Monthly | $39.20 · 2026-08-03 | active, price changed |
| Canva Pro | Software subscription | Monthly | $15.90 · 2026-07-28 | active, stable |
| Breezeway | Software subscription | Monthly | $49.98 · 2026-08-05 | active, stable |
| Xfinity (...4222) | Utility | Monthly | $55.00 · 2026-08-04 | active, stable |
| Xfinity (...6337) | Utility | Monthly | $70.90 · 2026-07-15 | active, stable |
| Apple Valley Waste | Utility | Quarterly | $253.90 · 2026-05-30 | active, price rising |
| QR Code Generator Pro | Software subscription | Unknown | $119.88 · 2026-08-05 | new, unconfirmed |
| Pool Pals, LLC | Service | Irregular | amount unknown · 2026-07-06 (last reminder) | active, frequently overdue |
| Petti Pest Control | Service | Irregular | amount unknown · 2026-08-03 (inspection report; last invoice 2026-07-14) | active |
| Booking.com (host invoices) | Platform commission | Irregular | amount unknown · 2026-07-06 (last invoice) | active, 2 listings |

Full history and machine-readable detail: `ledger/vendors.json`.
Paused-project list: `ledger/paused_projects.json`.
Process this file is generated from: `ledger/RUNBOOK.md`.
