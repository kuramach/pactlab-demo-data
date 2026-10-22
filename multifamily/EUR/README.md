# Larkfield Residential B.V. — Multifamily (EUR)

**Fictional target.** Larkfield Residential B.V. owns Larkfield Commons, a 96-unit garden-style apartment community in three buildings (A, B, C).
Based in Utrecht, the Netherlands; reports in EUR. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Files

| File | What it is | Load it in Pactlab |
|---|---|---|
| `invoice-lines.csv` | 2232 revenue lines, one per unit rent charge per month | Sources → Upload billing export → **Pactlab standard template** |
| `rent-roll.csv` | Rent roll at 30 September 2026 | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `delinquency.csv` | Delinquent balances at 30 September 2026 | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `unit-inspections.csv` | Unit-condition inspections with repair estimates | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `t12.csv` | Trailing-twelve-month operating statement (T-12) | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `documents/01-offering-memorandum.pdf` (`.md` source) | Offering memorandum with stated NOI and capital plan | Documents → upload, data class *Business* |
| `vdr-index.csv` | Index of every file, as a data room would list it | Reference |

## Demo walkthrough

1. **Start a Pact** for `Larkfield Residential B.V.` with base currency **EUR**, industry *Multifamily*.
2. **Sources → Upload billing export** → Pactlab standard template → `invoice-lines.csv` → Preview → Import. **Finances** shows the revenue ledger.
3. **Documents** → upload every PDF in `documents/` with the data class shown above.
4. Look for the planted findings below; accept, reject or ask for support, then price the accepted ones in **Valuation**.

## Planted findings

1. **Offering memorandum NOI above the T-12** — the memorandum states EUR 1,138,721; `t12.csv` sums to EUR 1,025,875 — the memorandum uses pro-forma rents.
2. **Deferred maintenance above the capital plan** — `unit-inspections.csv` estimates EUR 230,000 of repairs against a EUR 132,480 capital plan — EUR 2,396 per door. Price as remediation.
3. **Delinquency concentrated in Building C** — 90.0% of delinquent units in `delinquency.csv` are in Building C.
4. **Loss-to-lease (upside, not price)** — occupied units are 7.4% below market rent in `rent-roll.csv`. Record it as confirmed value — never as a reason to pay more.

## Notes

- Residents are referred to by unit only; there are no personal names.
- The rent roll maps onto the billing import: each occupied unit is a customer billed monthly.
