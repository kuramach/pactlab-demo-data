# Larkfield Residential Inc. — Multifamily (USD)

**Fictional target.** Larkfield Residential Inc. owns Larkfield Commons, a 96-unit garden-style apartment community in three buildings (A, B, C).
Based in Columbus, Ohio, United States; reports in USD. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Files

| File | What it is | Load it in Pactlab |
|---|---|---|
| `invoice-lines.csv` | 2280 revenue lines, one per unit rent charge per month | Sources → Upload billing export → **Pactlab standard template** |
| `rent-roll.csv` | Rent roll at 30 September 2026 | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `delinquency.csv` | Delinquent balances at 30 September 2026 | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `unit-inspections.csv` | Unit-condition inspections with repair estimates | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `t12.csv` | Trailing-twelve-month operating statement (T-12) | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `documents/01-offering-memorandum.pdf` (`.md` source) | Offering memorandum with stated NOI and capital plan | Documents → upload, data class *Business* |
| `vdr-index.csv` | Index of every file, as a data room would list it | Reference |

## Demo walkthrough

1. **Start a Pact** for `Larkfield Residential Inc.` with base currency **USD**, industry *Multifamily*.
2. **Sources → Upload billing export** → Pactlab standard template → `invoice-lines.csv` → Preview → Import. **Finances** shows the revenue ledger.
3. **Documents** → upload every PDF in `documents/` with the data class shown above.
4. Look for the planted findings below; accept, reject or ask for support, then price the accepted ones in **Valuation**.

## Planted findings

1. **Offering memorandum NOI above the T-12** — the memorandum states USD 1,299,489; `t12.csv` sums to USD 1,170,711 — the memorandum uses pro-forma rents.
2. **Deferred maintenance above the capital plan** — `unit-inspections.csv` estimates USD 232,100 of repairs against a USD 144,000 capital plan — USD 2,418 per door. Price as remediation.
3. **Delinquency concentrated in Building C** — 100.0% of delinquent units in `delinquency.csv` are in Building C.
4. **Loss-to-lease (upside, not price)** — occupied units are 6.9% below market rent in `rent-roll.csv`. Record it as confirmed value — never as a reason to pay more.

## Notes

- Residents are referred to by unit only; there are no personal names.
- The rent roll maps onto the billing import: each occupied unit is a customer billed monthly.
