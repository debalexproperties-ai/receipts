# Receipts Ledger — Weekly Digest

_Last updated: 2026-08-05 (initial backfill)_

## New charges this run
Initial backfill only - see `ledger/vendors.json` for the full ~150-message
history pulled from Sep 2025 through 2026-08-05. Going forward this section
lists only what showed up in the most recent `label:Receipts newer_than:8d`
search.

## Current confirmed monthly recurring total: **$230.98/mo**
PriceLabs $39.20 + Canva Pro $15.90 + Breezeway $49.98 + Xfinity ...4222
$55.00 + Xfinity ...6337 $70.90. Excludes QR Code Generator Pro (cycle not
yet confirmed monthly), Apple Valley Waste (quarterly), and Pool Pals /
Petti Pest Control / Booking.com (irregular, amount unknown).

## 🚩 Flags

| Flag | Vendor | Detail |
|---|---|---|
| **New vendor** | QR Code Generator Pro | First-ever charge, 2026-08-05: **$119.88**. Not seen anywhere else in the past year. Likely an annual plan - confirm this was intentional. |
| **Price change** | PriceLabs | Monthly charge rose from **$37.08 → $39.20** (+5.7%) starting the 2026-06-15 cycle, held through 2026-08-03. Nine months stable at $37.08 before that. |
| **Price trend** | Apple Valley Waste | Two consecutive increases: $228.58 → $241.00 → $253.90 (~+5.3-5.4% each). Worth confirming this is a published rate increase. |
| **Needs manual amounts** | Pool Pals, Petti Pest Control, Booking.com (host invoices) | Dollar amounts live in a PDF attachment or an external portal - this automation can log the occurrence but not the amount. |
| **Operational note** | Pool Pals | Mostly "OVERDUE"/"URGENT" reminders rather than fresh invoices - a slow-pay pattern independent of pricing. |

No duplicate-subscription and no paused-project flags yet (paused list is
currently empty - see `ledger/paused_projects.json`).

## Vendors tracked

| Vendor | Category | Billing cycle | Last known charge | Status |
|---|---|---|---|---|
| PriceLabs | Software subscription | Monthly | $39.20 · 2026-08-03 | active, price changed |
| Canva Pro | Software subscription | Monthly | $15.90 · 2026-07-28 | active, stable |
| Breezeway | Software subscription | Monthly | $49.98 · 2026-07-07 | active, stable |
| Xfinity (...4222) | Utility | Monthly | $55.00 · 2026-08-04 | active, stable |
| Xfinity (...6337) | Utility | Monthly | $70.90 · 2026-07-15 | active, stable |
| Apple Valley Waste | Utility | Quarterly | $253.90 · 2026-05-30 | active, price rising |
| QR Code Generator Pro | Software subscription | Unknown | $119.88 · 2026-08-05 | **new** |
| Pool Pals, LLC | Service | Irregular | amount unknown · 2026-07-06 (last reminder) | active, frequently overdue |
| Petti Pest Control | Service | Irregular | amount unknown · 2026-07-14 (last invoice) | active |
| Booking.com (host invoices) | Platform commission | Irregular | amount unknown · 2026-07-06 (last invoice) | active, 2 listings |

Full history and machine-readable detail: `ledger/vendors.json`.
Paused-project list: `ledger/paused_projects.json`.
Process this file is generated from: `ledger/RUNBOOK.md`.
