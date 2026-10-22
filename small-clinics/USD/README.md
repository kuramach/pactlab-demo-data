# Clearbrook Clinics Inc. — Small clinics (USD)

**Fictional target.** Clearbrook Clinics Inc. runs six dental and physiotherapy clinics with 22 providers, paid by insurers and patients.
Based in Columbus, Ohio, United States; reports in USD. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Files

| File | What it is | Load it in Pactlab |
|---|---|---|
| `invoice-lines.csv` | 96 revenue lines, one per payer remittance per month | Sources → Upload billing export → **Pactlab standard template** |
| `patient-volume.csv` | Visits and revenue by site and pseudonymous provider | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `equipment-schedule.csv` | Equipment with acquisition dates and useful lives | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `coding-summary.csv` | Share of visits billed at the highest complexity code | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `documents/01-coding-policy.pdf` (`.md` source) | Coding and billing policy | Documents → upload, data class *Business* |
| `vdr-index.csv` | Index of every file, as a data room would list it | Reference |

## Demo walkthrough

1. **Start a Pact** for `Clearbrook Clinics Inc.` with base currency **USD**, industry *Small clinics*.
2. **Sources → Upload billing export** → Pactlab standard template → `invoice-lines.csv` → Preview → Import. **Finances** shows the revenue ledger.
3. **Documents** → upload every PDF in `documents/` with the data class shown above.
4. Look for the planted findings below; accept, reject or ask for support, then price the accepted ones in **Valuation**.

## Planted findings

1. **One provider carries Site 3** — P07 earns 73.8% of Site 3 revenue in `patient-volume.csv` — a retention risk after closing.
2. **High-complexity coding above policy** — `coding-summary.csv` shows 31–36% of visits at the highest code against the 15% expected by `documents/01-coding-policy.pdf`.
3. **Imaging equipment past its useful life** — two panoramic X-ray units in `equipment-schedule.csv` (2014 and 2015, ten-year lives). Price as remediation.

## Notes

- Providers are pseudonymous (P01, P02, …); Pactlab never sends people data to a model.
