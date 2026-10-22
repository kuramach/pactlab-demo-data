# Harbourview Hotel Holdings B.V. — Hotels and hospitality (EUR)

**Fictional target.** Harbourview Hotel Holdings B.V. owns and operates the 180-room Harbourview Hotel, a branded upscale hotel under a franchise agreement.
Based in Utrecht, the Netherlands; reports in EUR. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Files

| File | What it is | Load it in Pactlab |
|---|---|---|
| `invoice-lines.csv` | 120 revenue lines, one per revenue-channel settlement per month | Sources → Upload billing export → **Pactlab standard template** |
| `operating-history.csv` | Monthly operating history from the property-management system | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `str-benchmark.csv` | STR-style benchmark against the competitive set | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `documents/01-franchise-agreement.pdf` (`.md` source) | Franchise agreement with transfer and PIP clauses | Documents → upload, data class *Business* |
| `documents/02-management-contract.pdf` (`.md` source) | Third-party management contract | Documents → upload, data class *Business* |
| `vdr-index.csv` | Index of every file, as a data room would list it | Reference |

## Demo walkthrough

1. **Start a Pact** for `Harbourview Hotel Holdings B.V.` with base currency **EUR**, industry *Hotels and hospitality*.
2. **Sources → Upload billing export** → Pactlab standard template → `invoice-lines.csv` → Preview → Import. **Finances** shows the revenue ledger.
3. **Documents** → upload every PDF in `documents/` with the data class shown above.
4. Look for the planted findings below; accept, reject or ask for support, then price the accepted ones in **Valuation**.

## Planted findings

1. **Brand PIP required on change of ownership** — `documents/01-franchise-agreement.pdf` page 2, clause 16.4 — PIP estimated at EUR 3,312,000. Price as remediation or escrow.
2. **RevPAR trailing the competitive set** — in `str-benchmark.csv` the hotel's RevPAR trails the competitive set by about 7% in October 2025, widening to about 12% by September 2026.
3. **Channel concentration** — BookNest online travel agency (synthetic) is 41.0% of revenue — commission cost and ranking risk.
4. **Seasonal demand** — July and August room revenue is about twice January's in `operating-history.csv`.
5. **Management contract termination fee** — `documents/02-management-contract.pdf` page 2, clause 12.2 — three times the prior year's base fee on sale.
