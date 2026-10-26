# Harbourview Hotel Holdings B.V. — Hotels and hospitality (EUR)

**Fictional target.** Harbourview Hotel Holdings B.V. owns and operates the 180-room Harbourview Hotel, a branded upscale hotel under a franchise agreement.
Based in Utrecht, the Netherlands; reports in EUR. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Before you start

- Download this whole folder (on GitHub: **Code → Download ZIP** at the top of the repository, then unzip).
- Sign in to Pactlab. The steps take about 15 minutes.
- You upload **3 CSV files** and **3 PDFs**. Nothing else.
- **Never upload the `.md` files** in `documents/`. They are the text each PDF is built from; Pactlab reads the PDFs.
- `vdr-index.csv` is for reference only (how a data room would list these files). Do not upload it.
- Text in **bold** below is a button, tab or option exactly as Pactlab shows it.

## Step 1 — Start the Pact

1. Click **Start a Pact** (top right).
2. **Name the Pact** — Pact name: `Project Harbourview` · Base currency: **EUR** → **Next**.
3. **Buying entity** — Legal or trading name: `Demo Buyer` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `Harbourview Hotel Holdings B.V.` · **Private** · What kind of company is it?: **Hotels & hospitality** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `27000000` (EUR 27,000,000) |
   | Currency | **EUR** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the seller's ask: 3.5× the September 2026 billed revenue run-rate. The demo shows how far the evidence supports it.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `Harbourview Hotel Holdings B.V.`, with the asking price EUR 27,000,000.

## Step 2 — Upload the billing export

1. Open the **Sources** tab → **Upload billing export**.
2. *1. Where is the export from?* → **Pactlab standard template**.
3. *2. Choose the file* → `invoice-lines.csv` → **Upload and map columns**.
4. The columns are matched for you. Click **Check every row**, then **Import 120 lines**.

**You should see:** a green message ending "Finances now include them." The **Finances** tab now shows the revenue ledger.

## Step 3 — Upload the industry data

Open the **Sources** tab and scroll to **Industry data**. Upload these files one at a time:

| # | Click | Choose the file | Then | Button should read |
|---|---|---|---|---|
| 1 | **Upload operating history** | `operating-history.csv` | **Upload and map columns** → **Check every row** | **Import 24 rows** |
| 2 | **Upload str benchmark** | `str-benchmark.csv` | **Upload and map columns** → **Check every row** | **Import 12 rows** |

**You should see** after each import: "… imported … Industry checks ran on them". Some findings may already appear as drafts; that is expected.

## Step 4 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/01-franchise-agreement.pdf` | **business information** | Franchise agreement with transfer and PIP clauses |
| 2 | `documents/02-management-contract.pdf` | **business information** | Third-party management contract |
| 3 | `documents/99-data-room-extracts.pdf` | **financial information** | Every CSV extract in this folder as one paged PDF, so findings can cite a page |

**You should see:** all 3 documents listed on the **Documents** tab.

## Step 5 — Run the checks and review the findings

1. Open the **Findings** tab → **Run hotels & hospitality checks**.
2. **You should see exactly these 5 findings** (running the checks again adds nothing):

   1. **Brand PIP required on change of ownership** — `documents/01-franchise-agreement.pdf` page 2, clause 16.4 — PIP estimated at EUR 3,312,000. Price as remediation or escrow.
   2. **RevPAR trailing the competitive set** — in `str-benchmark.csv` the hotel's RevPAR trails the competitive set by about 7% in October 2025, widening to about 12% by September 2026.
   3. **Channel concentration** — BookNest online travel agency (synthetic) is 41.0% of revenue — commission cost and ranking risk.
   4. **Seasonal demand** — July and August room revenue is about twice January's in `operating-history.csv`.
   5. **Management contract termination fee** — `documents/02-management-contract.pdf` page 2, clause 12.2 — three times the prior year's base fee on sale.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 6 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 120 revenue lines, one per revenue-channel settlement per month | **Yes** — billing export step |
| `operating-history.csv` | Monthly operating history from the property-management system (24 rows) | **Yes** — industry data step |
| `str-benchmark.csv` | STR-style benchmark against the competitive set (12 rows) | **Yes** — industry data step |
| `documents/01-franchise-agreement.pdf` | Franchise agreement with transfer and PIP clauses | **Yes** — documents step |
| `documents/02-management-contract.pdf` | Third-party management contract | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |
