# Riverside Care Partners B.V. — Healthcare services and healthtech (EUR)

**Fictional target.** Riverside Care Partners B.V. operates nine physical-therapy and primary-care practices, paid mostly by government programmes and commercial insurers.
Based in Utrecht, the Netherlands; reports in EUR. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Files

| File | What it is | Load it in Pactlab |
|---|---|---|
| `invoice-lines.csv` | 144 revenue lines, one per payer remittance per month | Sources → Upload billing export → **Pactlab standard template** |
| `claims-summary.csv` | Monthly claims billed, paid and denial rate by payer | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `provider-roster.csv` | Provider roster, pseudonymous, with credential expiry dates | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `documents/01-medical-director-agreement.pdf` (`.md` source) | Medical-director agreement and time records | Documents → upload, data class *Business* |
| `documents/02-privacy-risk-assessment.pdf` (`.md` source) | Most recent privacy and security risk assessment | Documents → upload, data class *Business* |
| `vdr-index.csv` | Index of every file, as a data room would list it | Reference |

## Demo walkthrough

1. **Start a Pact** for `Riverside Care Partners B.V.` with base currency **EUR**, industry *Healthcare services and healthtech*.
2. **Sources → Upload billing export** → Pactlab standard template → `invoice-lines.csv` → Preview → Import. **Finances** shows the revenue ledger.
3. **Documents** → upload every PDF in `documents/` with the data class shown above.
4. Look for the planted findings below; accept, reject or ask for support, then price the accepted ones in **Valuation**.

## Planted findings

1. **Revenue concentrated in government programmes** — government programmes A and B are 64.2% of September 2026 revenue in `invoice-lines.csv`.
2. **Medical-director fee above documented duties** — `documents/01-medical-director-agreement.pdf` — a fixed fee for four hours a month, against 1.5 documented hours (page 2).
3. **Privacy risk assessment out of date** — `documents/02-privacy-risk-assessment.pdf` — last assessed March 2023, review overdue since March 2024.
4. **Provider credentials expiring** — two providers in `provider-roster.csv` have credentials expiring before the end of 2026.

## Notes

- Provider data is pseudonymous and aggregate by design; Pactlab never sends people data to a model.
