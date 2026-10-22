# Brightwave Software Ltd — Software and SaaS (GBP)

**Fictional target.** Brightwave Software Ltd sells workflow software to mid-sized logistics and services firms on monthly and annual subscriptions.
Based in Leeds, the United Kingdom; reports in GBP. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Files

| File | What it is | Load it in Pactlab |
|---|---|---|
| `invoice-lines.csv` | 302 revenue lines, one per customer subscription per month | Sources → Upload billing export → **Pactlab standard template** |
| `documents/01-board-kpi-pack-2026-09.pdf` (`.md` source) | Management KPI pack with reported ARR | Documents → upload, data class *Business* |
| `documents/02-master-services-agreement-northgate.pdf` (`.md` source) | Largest customer contract, with change-of-control clause | Documents → upload, data class *Business* |
| `documents/03-balance-sheet-2026-09-30.pdf` (`.md` source) | Balance sheet with debt and debt-like items | Documents → upload, data class *Financial* |
| `vdr-index.csv` | Index of every file, as a data room would list it | Reference |

## Demo walkthrough

1. **Start a Pact** for `Brightwave Software Ltd` with base currency **GBP**, industry *Software and SaaS*.
2. **Sources → Upload billing export** → Pactlab standard template → `invoice-lines.csv` → Preview → Import. **Finances** shows the revenue ledger.
3. **Documents** → upload every PDF in `documents/` with the data class shown above.
4. Look for the planted findings below; accept, reject or ask for support, then price the accepted ones in **Valuation**.

## Planted findings

1. **Management ARR exceeds billed ARR** — the KPI pack reports GBP 518,328; `invoice-lines.csv` supports GBP 497,946 at September 2026 — a gap of GBP 20,382. The KPI pack still counts Quarry Lane Studios, whose last invoice was June 2026.
2. **Revenue concentration** — Harborline Freight (synthetic) is 27.6% of September 2026 billed revenue.
3. **Largest customer can leave on a sale** — `documents/02-master-services-agreement-northgate.pdf` page 2, clause 14 — termination on change of control.
4. **Contraction hidden in the logo count** — Amberline Hotels drops by 30% from April 2026; the KPI pack reports 14 active customers, the ledger has 13.

## Notes

- Code and delivery data (GitHub, Jira) connect through their APIs, not files: in a local or dev Pactlab, use **Sources → Connect synthetic code and Jira data**.
