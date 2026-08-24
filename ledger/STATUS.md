# Receipts Ledger — Weekly Digest

_Last updated: 2026-08-24_

## New charges this run
Searched `label:Receipts newer_than:8d` (7 threads found). One (Booking.com
"booking confirmed" for CITYLUXE Suites & Rooms, Athens) is Deb's personal
guest travel and out of scope for this ledger - excluded. **6 rows
appended**, all existing vendors, no price changes:

- **Xfinity (...6337)** — bill-available notice, **$70.90**, AutoPay
  scheduled for 2026-09-14. Same amount as last confirmed payment - no
  price change.
- **Pool Pals, LLC** — new invoice #1511 (2026-08-18, amount inside PDF
  attachment, not extracted) plus two overdue reminders for that same
  invoice (2026-08-19, 2026-08-20). A reply-thread exchange confirms both
  hot tubs were serviced (drained, cleaned, filled) - not a billing issue,
  just a service-scope question Deb asked and Pool Pals answered. This is
  the same slow-pay reminder pattern already noted for this vendor, not a
  new duplicate charge.
- **Petti Pest Control** — invoice #341342 (2026-08-21, amount inside PDF,
  property not stated in the email body) and a separate inspection report
  for 704 Valley View Rd (2026-08-21, informational, no charge).

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
- **Pool Pals, LLC** - continues its pattern of frequent overdue reminders
  (invoice #1511 got two reminders this run alone). Amounts still can't be
  confirmed (PDF attachments); worth a look if the slow-pay pattern is a
  concern beyond pricing.

## Vendors tracked

| Vendor | Category | Billing cycle | Last known charge | Status |
|---|---|---|---|---|
| PriceLabs | Software subscription | Monthly | $39.20 · 2026-08-03 | active, price changed |
| Canva Pro | Software subscription | Monthly | $15.90 · 2026-07-28 | active, stable |
| Breezeway | Software subscription | Monthly | $49.98 · 2026-08-05 | active, stable |
| Xfinity (...4222) | Utility | Monthly | $55.00 · 2026-08-12 (bill notice, AutoPay 2026-09-03) | active, stable |
| Xfinity (...6337) | Utility | Monthly | $70.90 · 2026-08-22 (bill notice, AutoPay 2026-09-14) | active, stable |
| Apple Valley Waste | Utility | Quarterly | $253.90 · 2026-05-30 | active, price rising |
| QR Code Generator Pro | Software subscription | Unknown | $119.88 · 2026-08-05 | new, unconfirmed |
| Pool Pals, LLC | Service | Irregular | amount unknown · 2026-08-20 (2nd reminder; invoice #1511 · 2026-08-18) | active, frequently overdue |
| Petti Pest Control | Service | Irregular | amount unknown · 2026-08-21 (invoice #341342; inspection report same day, 704 Valley View Rd) | active |
| Booking.com (host invoices) | Platform commission | Irregular | amount unknown · 2026-08-06 (last invoice) | active, 2 listings |
| Potomac Edison (...6615, 1030 Shannondale) | Utility | Monthly | $158.74 · 2026-08-07 (statement) | new, unconfirmed |
| Potomac Edison (...8822, 704 Valley View) | Utility | Monthly | $202.36 · 2026-08-06 (statement) | new, unconfirmed |

Full history and machine-readable detail: `ledger/vendors.json`.
Paused-project list: `ledger/paused_projects.json`.
Process this file is generated from: `ledger/RUNBOOK.md`.
