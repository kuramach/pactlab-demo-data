# Sablestone Consulting Ltd — IT and professional services (GBP)

**Fictional target.** Sablestone Consulting Ltd is a 140-person digital and data consultancy working on monthly retainers for enterprise clients.
Based in Leeds, the United Kingdom; reports in GBP. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Files

| File | What it is | Load it in Pactlab |
|---|---|---|
| `invoice-lines.csv` | 192 revenue lines, one per client retainer per month | Sources → Upload billing export → **Pactlab standard template** |
| `timesheets-summary.csv` | Available and billable hours by team (aggregate) | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `headcount-movements.csv` | Starters, leavers and headcount by role family (aggregate) | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `documents/01-management-pack-2026-09.pdf` (`.md` source) | Management pack with reported utilization | Documents → upload, data class *Business* |
| `documents/02-msa-meridian.pdf` (`.md` source) | Master services agreement with the largest client | Documents → upload, data class *Business* |
| `vdr-index.csv` | Index of every file, as a data room would list it | Reference |

## Demo walkthrough

1. **Start a Pact** for `Sablestone Consulting Ltd` with base currency **GBP**, industry *IT and professional services*.
2. **Sources → Upload billing export** → Pactlab standard template → `invoice-lines.csv` → Preview → Import. **Finances** shows the revenue ledger.
3. **Documents** → upload every PDF in `documents/` with the data class shown above.
4. Look for the planted findings below; accept, reject or ask for support, then price the accepted ones in **Valuation**.

## Planted findings

1. **Utilization below the reported level** — the management pack reports 78%; `timesheets-summary.csv` gives 64.2% over the last twelve months.
2. **Largest client terminable for convenience** — Meridian Retail Group (synthetic) is 37.8% of September 2026 revenue and can terminate on sixty days' notice (`documents/02-msa-meridian.pdf` page 2, clause 18.2).
3. **Rising attrition in delivery roles** — monthly delivery leavers rise from 1 to 4 across the year in `headcount-movements.csv`.

## Notes

- People data is aggregate only — no names, no individual records.
