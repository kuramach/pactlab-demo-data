# St. Brennan Health Inc. — Hospitals (USD)

**Fictional target.** St. Brennan Health Inc. operates St. Brennan Regional Medical Center, a 220-bed acute-care hospital with cardiology, orthopaedics and maternity service lines.
Based in Columbus, Ohio, United States; reports in USD. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Files

| File | What it is | Load it in Pactlab |
|---|---|---|
| `invoice-lines.csv` | 120 revenue lines, one per payer net-revenue settlement per month | Sources → Upload billing export → **Pactlab standard template** |
| `census.csv` | Admissions and census by service line | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `payer-mix.csv` | Gross charges and net revenue by payer | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `documents/01-accreditation-record.pdf` (`.md` source) | Accreditation record and transfer condition | Documents → upload, data class *Business* |
| `documents/02-medicare-cost-report-summary.pdf` (`.md` source) | Cost report summary with committed regulatory capex | Documents → upload, data class *Financial* |
| `documents/03-service-line-dependence.pdf` (`.md` source) | Aggregate physician dependence by service line | Documents → upload, data class *Business* |
| `vdr-index.csv` | Index of every file, as a data room would list it | Reference |

## Demo walkthrough

1. **Start a Pact** for `St. Brennan Health Inc.` with base currency **USD**, industry *Hospitals*.
2. **Sources → Upload billing export** → Pactlab standard template → `invoice-lines.csv` → Preview → Import. **Finances** shows the revenue ledger.
3. **Documents** → upload every PDF in `documents/` with the data class shown above.
4. Look for the planted findings below; accept, reject or ask for support, then price the accepted ones in **Valuation**.

## Planted findings

1. **Earnings concentrated in one payer** — Government programme A (synthetic) is 56.7% of September 2026 net revenue.
2. **Accreditation does not transfer automatically** — `documents/01-accreditation-record.pdf` page 2 — make it a closing condition.
3. **Key-physician dependence in cardiology** — `documents/03-service-line-dependence.pdf` — two physicians perform about 80% of cardiology procedures (aggregate data only).
4. **Committed regulatory capex** — `documents/02-medicare-cost-report-summary.pdf` — USD 4,100,000 committed. Price as remediation.

## Notes

- Physician data is aggregate only; Pactlab never sends people data to a model.
