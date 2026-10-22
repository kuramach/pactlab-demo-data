# Quayside Estates B.V. — Commercial property (EUR)

**Fictional target.** Quayside Estates B.V. owns Quayside Business Park, a 210,000 sq ft mixed office and light-industrial park with eleven tenants.
Based in Utrecht, the Netherlands; reports in EUR. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Files

| File | What it is | Load it in Pactlab |
|---|---|---|
| `invoice-lines.csv` | 264 revenue lines, one per tenant base-rent charge per month | Sources → Upload billing export → **Pactlab standard template** |
| `rent-roll.csv` | Commercial rent roll with expiries and market rents | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `cam-reconciliation.csv` | Common-area-maintenance expenses against tenant recoveries | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `documents/01-phase-i-environmental-site-assessment.pdf` (`.md` source) | Phase I environmental site assessment | Documents → upload, data class *Business* |
| `documents/02-lease-abstract-corvane.pdf` (`.md` source) | Lease abstract for the anchor tenant | Documents → upload, data class *Business* |
| `vdr-index.csv` | Index of every file, as a data room would list it | Reference |

## Demo walkthrough

1. **Start a Pact** for `Quayside Estates B.V.` with base currency **EUR**, industry *Commercial property*.
2. **Sources → Upload billing export** → Pactlab standard template → `invoice-lines.csv` → Preview → Import. **Finances** shows the revenue ledger.
3. **Documents** → upload every PDF in `documents/` with the data class shown above.
4. Look for the planted findings below; accept, reject or ask for support, then price the accepted ones in **Valuation**.

## Planted findings

1. **Anchor tenant concentration and near-term expiry** — Corvane Logistics (synthetic) is 41.0% of base rent and its lease ends 30 June 2027 (`rent-roll.csv`, `documents/02-lease-abstract-corvane.pdf`). Weighted average lease term is 2.3 years.
2. **Recognized environmental condition** — `documents/01-phase-i-environmental-site-assessment.pdf` page 2 — former dry cleaner at Unit 9; Phase II recommended.
3. **CAM recoveries below expenses** — `cam-reconciliation.csv` — repairs and security recover less than they cost.
4. **Below-market anchor rent** — Corvane pays about 6% below market rent in `rent-roll.csv` — the deepest discount on the rent roll, on the largest lease.
