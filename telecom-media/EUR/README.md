# Northlake Fibre B.V. — Telecom and media (EUR)

**Fictional target.** Northlake Fibre B.V. is a regional fibre broadband and streaming-TV provider selling residential and small-business plans in four regions.
Based in Utrecht, the Netherlands; reports in EUR. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Files

| File | What it is | Load it in Pactlab |
|---|---|---|
| `invoice-lines.csv` | 288 revenue lines, one per region-and-plan subscriber billing per month | Sources → Upload billing export → **Pactlab standard template** |
| `subscribers-by-month.csv` | Billed subscribers and ARPU by region and plan | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `documents/01-kpi-pack-2026-09.pdf` (`.md` source) | Management KPI pack with reported subscribers and churn | Documents → upload, data class *Business* |
| `documents/02-wholesale-network-agreement.pdf` (`.md` source) | Wholesale network access agreement | Documents → upload, data class *Business* |
| `vdr-index.csv` | Index of every file, as a data room would list it | Reference |

## Demo walkthrough

1. **Start a Pact** for `Northlake Fibre B.V.` with base currency **EUR**, industry *Telecom and media*.
2. **Sources → Upload billing export** → Pactlab standard template → `invoice-lines.csv` → Preview → Import. **Finances** shows the revenue ledger.
3. **Documents** → upload every PDF in `documents/` with the data class shown above.
4. Look for the planted findings below; accept, reject or ask for support, then price the accepted ones in **Valuation**.

## Planted findings

1. **Reported subscribers exceed billed subscribers** — the KPI pack reports 12,382; `subscribers-by-month.csv` bills 11,638 in September 2026.
2. **Churn rising in 2026** — billed subscribers grow about 0.3% a month until December 2025, then shrink about 0.5% a month from January 2026 (`invoice-lines.csv`, `subscribers-by-month.csv`); the KPI pack still reports 0.9% churn.
3. **Regional concentration** — the North region is 44.7% of September 2026 revenue.
4. **Wholesale price review ahead** — `documents/02-wholesale-network-agreement.pdf` page 2, clause 9 — next re-pricing 1 January 2027.
