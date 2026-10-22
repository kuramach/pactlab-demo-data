# Ridgeline Outfitters B.V. — E-commerce and DTC (EUR)

**Fictional target.** Ridgeline Outfitters B.V. sells outdoor apparel direct to consumers through its own store, one large marketplace and a few wholesale retailers.
Based in Utrecht, the Netherlands; reports in EUR. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Files

| File | What it is | Load it in Pactlab |
|---|---|---|
| `invoice-lines.csv` | 96 revenue lines, one per sales-channel payout per month | Sources → Upload billing export → **Pactlab standard template** |
| `orders-by-cohort.csv` | Repeat purchase by first-purchase cohort | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `ad-spend.csv` | Advertising spend and new customers by channel | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `documents/01-marketplace-seller-terms.pdf` (`.md` source) | Marketplace seller terms | Documents → upload, data class *Business* |
| `vdr-index.csv` | Index of every file, as a data room would list it | Reference |

## Demo walkthrough

1. **Start a Pact** for `Ridgeline Outfitters B.V.` with base currency **EUR**, industry *E-commerce and DTC*.
2. **Sources → Upload billing export** → Pactlab standard template → `invoice-lines.csv` → Preview → Import. **Finances** shows the revenue ledger.
3. **Documents** → upload every PDF in `documents/` with the data class shown above.
4. Look for the planted findings below; accept, reject or ask for support, then price the accepted ones in **Valuation**.

## Planted findings

1. **Majority of revenue through one marketplace** — Marketvale marketplace payouts (synthetic) is 56.8% of September 2026 revenue.
2. **Repeat purchase declining in recent cohorts** — `orders-by-cohort.csv` — cohorts from 2025-07 keep about 27% of customers in their second month, against about 39% for earlier cohorts.
3. **Acquisition cost rising on paid social** — `ad-spend.csv` — paid-social spend rises every month while new customers fall.
