# Calvera Pharmaceuticals Inc. — Pharma and biotech (USD)

**Fictional target.** Calvera Pharmaceuticals Inc. is a specialty-pharma company earning royalties and supply revenue on two marketed products, with one late-stage programme.
Based in Columbus, Ohio, United States; reports in USD. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Files

| File | What it is | Load it in Pactlab |
|---|---|---|
| `invoice-lines.csv` | 96 revenue lines, one per partner royalty and supply payment per month | Sources → Upload billing export → **Pactlab standard template** |
| `patent-schedule.csv` | Patent families, products and expiry dates | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `pipeline.csv` | Development pipeline and next milestones | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `documents/01-revenue-forecast.pdf` (`.md` source) | Management revenue forecast and its exclusivity assumption | Documents → upload, data class *Business* |
| `documents/02-supplier-inspection-report.pdf` (`.md` source) | Contract manufacturer inspection summary | Documents → upload, data class *Business* |
| `vdr-index.csv` | Index of every file, as a data room would list it | Reference |

## Demo walkthrough

1. **Start a Pact** for `Calvera Pharmaceuticals Inc.` with base currency **USD**, industry *Pharma and biotech*.
2. **Sources → Upload billing export** → Pactlab standard template → `invoice-lines.csv` → Preview → Import. **Finances** shows the revenue ledger.
3. **Documents** → upload every PDF in `documents/` with the data class shown above.
4. Look for the planted findings below; accept, reject or ask for support, then price the accepted ones in **Valuation**.

## Planted findings

1. **Key patent expires earlier than the forecast assumes** — the forecast assumes exclusivity through 2031; `patent-schedule.csv` shows the Product A composition-of-matter patents expiring in 2028.
2. **Open manufacturing observations at the supplier** — `documents/02-supplier-inspection-report.pdf` page 2 — three open observations.
3. **Partner concentration** — Aldermoor Therapeutics accounts for both of the two largest revenue lines; the royalty line alone is 58.2% of September 2026 revenue.
