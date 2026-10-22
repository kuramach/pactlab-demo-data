# Tallyport Payments Inc. — Fintech (USD)

**Fictional target.** Tallyport Payments Inc. runs a payments and working-capital platform for independent retailers, earning monthly platform fees and lending to merchants through a partner bank.
Based in Columbus, Ohio, United States; reports in USD. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Files

| File | What it is | Load it in Pactlab |
|---|---|---|
| `invoice-lines.csv` | 328 revenue lines, one per merchant platform fee per month | Sources → Upload billing export → **Pactlab standard template** |
| `loan-tape.csv` | Loan-level tape for merchant working-capital loans | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `aml-alerts.csv` | Transaction-monitoring alerts and whether review evidence exists | Documents → upload `documents/99-data-room-extracts.pdf` (this table is on its own page) |
| `documents/01-balance-sheet-2026-09-30.pdf` (`.md` source) | Balance sheet extract with the credit-loss allowance | Documents → upload, data class *Financial* |
| `documents/02-aml-procedure.pdf` (`.md` source) | Written AML alert-handling procedure | Documents → upload, data class *Business* |
| `documents/03-partner-bank-agreement.pdf` (`.md` source) | Partner-bank program agreement | Documents → upload, data class *Business* |
| `vdr-index.csv` | Index of every file, as a data room would list it | Reference |

## Demo walkthrough

1. **Start a Pact** for `Tallyport Payments Inc.` with base currency **USD**, industry *Fintech*.
2. **Sources → Upload billing export** → Pactlab standard template → `invoice-lines.csv` → Preview → Import. **Finances** shows the revenue ledger.
3. **Documents** → upload every PDF in `documents/` with the data class shown above.
4. Look for the planted findings below; accept, reject or ask for support, then price the accepted ones in **Valuation**.

## Planted findings

1. **Allowance below observed loss experience** — the balance sheet carries a 2.0% allowance (USD 15,567); `loan-tape.csv` shows charge-offs of 13.5% of originated principal.
2. **Alerts closed without review evidence** — 24 of 80 closed alerts in `aml-alerts.csv` have `review_evidence = no`, against the procedure in `documents/02-aml-procedure.pdf`.
3. **Partner bank can terminate on change of control** — `documents/03-partner-bank-agreement.pdf` page 2, clause 22.3 — consent needed before closing.
