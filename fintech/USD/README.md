# Tallyport Payments Inc. — Fintech (USD)

**Fictional target.** Tallyport Payments Inc. runs a payments and working-capital platform for independent retailers, earning monthly platform fees and lending to merchants through a partner bank.
Based in Columbus, Ohio, United States; reports in USD. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Before you start

- Download this whole folder (on GitHub: **Code → Download ZIP** at the top of the repository, then unzip).
- Sign in to Pactlab. The steps take about 15 minutes.
- You upload **3 CSV files** and **4 PDFs**. Nothing else.
- **Never upload the `.md` files** in `documents/`. They are the text each PDF is built from; Pactlab reads the PDFs.
- `vdr-index.csv` is for reference only (how a data room would list these files). Do not upload it.
- Text in **bold** below is a button, tab or option exactly as Pactlab shows it.

## Step 1 — Start the Pact

1. Click **Start a Pact** (top right).
2. **Name the Pact** — Pact name: `Project Tallyport` · Base currency: **USD** → **Next**.
3. **Buying entity** — Legal or trading name: `Demo Buyer` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `Tallyport Payments Inc.` · **Private** · What kind of company is it?: **Fintech** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `3100000` (USD 3,100,000) |
   | Currency | **USD** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the seller's ask: 4× the September 2026 billed revenue run-rate. The demo shows how far the evidence supports it.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `Tallyport Payments Inc.`, with the asking price USD 3,100,000.

## Step 2 — Upload the billing export

1. Open the **Sources** tab → **Upload billing export**.
2. *1. Where is the export from?* → **Pactlab standard template**.
3. *2. Choose the file* → `invoice-lines.csv` → **Upload and map columns**.
4. The columns are matched for you. Click **Check every row**, then **Import 328 lines**.

**You should see:** a green message ending "Finances now include them." The **Finances** tab now shows the revenue ledger.

## Step 3 — Upload the industry data

Open the **Sources** tab and scroll to **Industry data**. Upload these files one at a time:

| # | Click | Choose the file | Then | Button should read |
|---|---|---|---|---|
| 1 | **Upload loan tape** | `loan-tape.csv` | **Upload and map columns** → **Check every row** | **Import 120 rows** |
| 2 | **Upload aml alerts** | `aml-alerts.csv` | **Upload and map columns** → **Check every row** | **Import 80 rows** |

**You should see** after each import: "… imported … Industry checks ran on them". Some findings may already appear as drafts; that is expected.

## Step 4 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/01-balance-sheet-2026-09-30.pdf` | **financial information** | Balance sheet extract with the credit-loss allowance |
| 2 | `documents/02-aml-procedure.pdf` | **business information** | Written AML alert-handling procedure |
| 3 | `documents/03-partner-bank-agreement.pdf` | **business information** | Partner-bank program agreement |
| 4 | `documents/99-data-room-extracts.pdf` | **financial information** | Every CSV extract in this folder as one paged PDF, so findings can cite a page |

**You should see:** all 4 documents listed on the **Documents** tab.

## Step 5 — Run the checks and review the findings

1. Open the **Findings** tab → **Run fintech checks**.
2. **You should see exactly these 3 findings** (running the checks again adds nothing):

   1. **Allowance below observed loss experience** — the balance sheet carries a 2.0% allowance (USD 15,567); `loan-tape.csv` shows charge-offs of 13.5% of originated principal.
   2. **Alerts closed without review evidence** — 24 of 80 closed alerts in `aml-alerts.csv` have `review_evidence = no`, against the procedure in `documents/02-aml-procedure.pdf`.
   3. **Partner bank can terminate on change of control** — `documents/03-partner-bank-agreement.pdf` page 2, clause 22.3 — consent needed before closing.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 6 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 328 revenue lines, one per merchant platform fee per month | **Yes** — billing export step |
| `loan-tape.csv` | Loan-level tape for merchant working-capital loans (120 rows) | **Yes** — industry data step |
| `aml-alerts.csv` | Transaction-monitoring alerts and whether review evidence exists (80 rows) | **Yes** — industry data step |
| `documents/01-balance-sheet-2026-09-30.pdf` | Balance sheet extract with the credit-loss allowance | **Yes** — documents step |
| `documents/02-aml-procedure.pdf` | Written AML alert-handling procedure | **Yes** — documents step |
| `documents/03-partner-bank-agreement.pdf` | Partner-bank program agreement | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |
