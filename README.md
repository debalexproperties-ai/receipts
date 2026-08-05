# weeklyreport

A Gmail-connected receipts ledger for deb.alex.properties@gmail.com.

Every week, an automated session scans the **Receipts** Gmail label, updates
a running ledger of vendor charges, and flags:

- **New vendors** — a charge from a sender never seen before
- **Price changes** — a recurring vendor's amount moved
- **Duplicate charges/subscriptions** — the same vendor billed twice
  unexpectedly, or two vendors serving the same purpose

Start here:

- [`ledger/STATUS.md`](ledger/STATUS.md) — current flags and vendor summary, human-readable
- [`ledger/vendors.json`](ledger/vendors.json) — full machine-readable ledger and charge history
- [`ledger/RUNBOOK.md`](ledger/RUNBOOK.md) — exact steps the weekly automation follows

The weekly run is a scheduled Routine (Mondays ~7am ET) that emails a
summary to deb.alex.properties@gmail.com and pushes ledger updates to this
branch.
