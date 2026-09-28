# Receipts Ledger — Weekly Digest

_Last updated: 2026-09-28_

## New charges this run
Searched `label:Receipts newer_than:8d` (4 threads / 4 messages found, all
new - deduped against every `message_id` already in the ledger). Rows
appended across 4 vendors:

- **Anthropic (Claude Pro)** — $21.40 receipt, 2026-09-26 (Receipt
  #2346-9438-4882, billing period Sep 26-Oct 26). Same price as the first
  charge last month - **second consecutive month confirms this as a real
  recurring subscription**, so it's promoted from "new" to "active" and
  now counted in the monthly burn total for the first time.
- **Xfinity (...6337)** — $70.90 bill statement, 2026-09-23. AutoPay
  scheduled for 2026-10-14, not yet a confirmed completed charge. Same
  amount as last month - no price change.
- **Petti Pest Control** — one inspection report at 1030 Shannondale Rd
  (2026-09-23, no charge, informational only).
- **Pool Pals, LLC** — one more overdue reminder for invoice #1511
  (2026-09-21, now **34 days overdue**), bringing that single still-open
  invoice to **13** reminders since it opened 2026-08-18. Balance
  confirmed again at **$498.20**. This reminder escalated to "URGENT"
  language.

## Current confirmed monthly recurring total: **$636.08/mo**
Up from $614.68 last week - **Anthropic (Claude Pro) $21.40/mo** is now
included for the first time, since a second consecutive charge confirms
it's a real recurring cost, not a one-off: PriceLabs $39.20 + Canva Pro
$15.90 + Breezeway $49.98 + Xfinity ...4222 $55.00 + Xfinity ...6337
$70.90 + Potomac Edison ...6615 $189.75 + Potomac Edison ...8822 $193.95
+ Anthropic (Claude Pro) $21.40.

## 🚩 Flags

**No new-vendor, price-change, duplicate-subscription/charge, or
paused-project flags this week** (paused list is still empty - see
`ledger/paused_projects.json`). Two things worth your attention anyway:

- **Pool Pals invoice #1511 slow-pay streak keeps escalating, now 34 days
  overdue.** **13** overdue reminders total (08-19 through 09-21) with no
  new invoice in between, balance still confirmed at **$498.20**. This
  week's reminder shifted to "URGENT" wording - worth contacting Pool Pals
  directly to confirm whether this has actually been paid, since it's
  been over a month with no resolution either way.
- **Anthropic (Claude Pro) now confirmed recurring at $21.40/mo** and
  entering your monthly burn total for the first time - flagging in case
  this subscription wasn't intentional or is a duplicate of another AI
  tool (no overlap found with existing vendors, but worth a gut check).

Carried over from prior weeks, still worth a look if not already resolved:
- **QR Code Generator Pro** ($119.88, 2026-08-05) - new vendor, likely an
  annual plan. Confirm this was intentional.
- **PriceLabs** price change ($37.08 → $39.20, +5.7%) from 2026-06-15,
  confirmed steady through 2026-09-03.

## Vendors tracked

| Vendor | Category | Billing cycle | Last known charge | Status |
|---|---|---|---|---|
| PriceLabs | Software subscription | Monthly | $39.20 · 2026-09-03 | active, stable |
| Canva Pro | Software subscription | Monthly | $15.90 · 2026-08-28 | active, stable |
| Breezeway | Software subscription | Monthly | $49.98 · 2026-09-03 | active, stable |
| Xfinity (...4222) | Utility | Monthly | $55.00 · 2026-09-12 (bill notice, AutoPay 2026-10-03) | active, stable |
| Xfinity (...6337) | Utility | Monthly | $70.90 · 2026-09-23 (bill notice, AutoPay 2026-10-14) | active, stable |
| Apple Valley Waste | Utility | Quarterly | $251.10 · 2026-09-16 | active, price steady |
| QR Code Generator Pro | Software subscription | Unknown | $119.88 · 2026-08-05 | new, unconfirmed |
| Pool Pals, LLC | Service | Irregular | $498.20 · 2026-09-21 (13th reminder; invoice #1511 · 2026-08-18) | active, frequently overdue |
| Petti Pest Control | Service | Irregular | amount unknown · 2026-09-23 (inspection report) | active |
| Booking.com (host invoices) | Platform commission | Irregular | amount unknown · 2026-09-06 (last invoice) | active, 2 listings |
| Potomac Edison (...6615, 1030 Shannondale) | Utility | Monthly | $189.75 · 2026-09-04 (statement) | active, usage-based |
| Potomac Edison (...8822, 704 Valley View) | Utility | Monthly | $193.95 · 2026-09-04 (statement) | active, usage-based |
| Anthropic (Claude Pro) | Software subscription | Monthly | $21.40 · 2026-09-26 | active, confirmed recurring |

Full history and machine-readable detail: `ledger/vendors.json`.
Paused-project list: `ledger/paused_projects.json`.
Process this file is generated from: `ledger/RUNBOOK.md`.
