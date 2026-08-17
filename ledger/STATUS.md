# Receipts Ledger — Weekly Digest

_Last updated: 2026-08-17_

## New charges this run
Searched `label:Receipts newer_than:8d` (2 threads found, neither previously
seen). **2 new rows appended**, both existing Xfinity accounts, no price
changes:

- **Xfinity (...6337)** — confirmed payment **$70.90** on 2026-08-15
  ("Thanks for your payment").
- **Xfinity (...4222)** — bill-available notice, **$55.00**, AutoPay
  scheduled for 2026-09-03. This is an advance notice, not yet a confirmed
  completed charge (logged as type `statement`); same amount as last
  month, so no price change either way.

## Current confirmed monthly recurring total: **$230.98/mo**
Unchanged from last week: PriceLabs $39.20 + Canva Pro $15.90 + Breezeway
$49.98 + Xfinity ...4222 $55.00 + Xfinity ...6337 $70.90. Excludes QR Code
Generator Pro (cycle unconfirmed), Apple Valley Waste (quarterly), Pool
Pals/Petti Pest Control/Booking.com (irregular, amount unknown), and the
two Potomac Edison electric accounts (still status "new" - only one
statement each so far, $158.74 + $202.36 = $361.10/mo once a second month
confirms the pattern, which would raise the total to ~$592.08/mo).

## 🚩 Flags

**No flags this week.** No new vendors, no price changes, no duplicate
subscriptions or charges, and no charges tied to a paused project (paused
list is still empty - see `ledger/paused_projects.json`).

Carried over from prior weeks, still worth a look if not already resolved:
- **Potomac Edison** (both properties) - new vendor flagged 2026-08-10,
  one statement each so far ($158.74 1030 Shannondale + $202.36 704 Valley
  View). Still needs a second month's statement to confirm this is the
  steady recurring pattern before it's added to the confirmed monthly
  total.
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
| Xfinity (...4222) | Utility | Monthly | $55.00 · 2026-08-12 (bill notice, AutoPay 2026-09-03) | active, stable |
| Xfinity (...6337) | Utility | Monthly | $70.90 · 2026-08-15 | active, stable |
| Apple Valley Waste | Utility | Quarterly | $253.90 · 2026-05-30 | active, price rising |
| QR Code Generator Pro | Software subscription | Unknown | $119.88 · 2026-08-05 | new, unconfirmed |
| Pool Pals, LLC | Service | Irregular | amount unknown · 2026-07-06 (last reminder) | active, frequently overdue |
| Petti Pest Control | Service | Irregular | amount unknown · 2026-08-03 (inspection report; last invoice 2026-07-14) | active |
| Booking.com (host invoices) | Platform commission | Irregular | amount unknown · 2026-08-06 (last invoice) | active, 2 listings |
| Potomac Edison (...6615, 1030 Shannondale) | Utility | Monthly | $158.74 · 2026-08-07 (statement) | new, unconfirmed |
| Potomac Edison (...8822, 704 Valley View) | Utility | Monthly | $202.36 · 2026-08-06 (statement) | new, unconfirmed |

Full history and machine-readable detail: `ledger/vendors.json`.
Paused-project list: `ledger/paused_projects.json`.
Process this file is generated from: `ledger/RUNBOOK.md`.
