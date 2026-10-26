# Sablestone Consulting Inc. — IT and professional services (USD)

**Fictional target.** Sablestone Consulting Inc. is a 140-person digital and data consultancy working on monthly retainers for enterprise clients.
Based in Columbus, Ohio, United States; reports in USD. Data runs October 2024 to September 2026.

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
2. **Name the Pact** — Pact name: `Project Sablestone` · Base currency: **USD** → **Next**.
3. **Buying entity** — Legal or trading name: `Demo Buyer` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `Sablestone Consulting Inc.` · **Private** · What kind of company is it?: **Professional services** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `4800000` (USD 4,800,000) |
   | Currency | **USD** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the seller's ask: 1.2× the September 2026 billed revenue run-rate. The demo shows how far the evidence supports it.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `Sablestone Consulting Inc.`, with the asking price USD 4,800,000.

## Step 2 — Upload the billing export

1. Open the **Sources** tab → **Upload billing export**.
2. *1. Where is the export from?* → **Pactlab standard template**.
3. *2. Choose the file* → `invoice-lines.csv` → **Upload and map columns**.
4. The columns are matched for you. Click **Check every row**, then **Import 192 lines**.

**You should see:** a green message ending "Finances now include them." The **Finances** tab now shows the revenue ledger.

## Step 3 — Upload the industry data

Open the **Sources** tab and scroll to **Industry data**. Upload these files one at a time:

| # | Click | Choose the file | Then | Button should read |
|---|---|---|---|---|
| 1 | **Upload timesheets summary** | `timesheets-summary.csv` | **Upload and map columns** → **Check every row** | **Import 36 rows** |
| 2 | **Upload headcount movements** | `headcount-movements.csv` | **Upload and map columns** → **Check every row** | **Import 24 rows** |

**You should see** after each import: "… imported … Industry checks ran on them". Some findings may already appear as drafts; that is expected.

## Step 4 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/01-management-pack-2026-09.pdf` | **business information** | Management pack with reported utilization |
| 2 | `documents/02-msa-meridian.pdf` | **business information** | Master services agreement with the largest client |
| 3 | `documents/99-data-room-extracts.pdf` | **financial information** | Every CSV extract in this folder as one paged PDF, so findings can cite a page |

**You should see:** all 3 documents listed on the **Documents** tab.

## Step 5 — Run the checks and review the findings

1. Open the **Findings** tab → **Run professional services checks**.
2. **You should see exactly these 3 findings** (running the checks again adds nothing):

   1. **Utilization below the reported level** — the management pack reports 78%; `timesheets-summary.csv` gives 64.7% over the last twelve months.
   2. **Largest client terminable for convenience** — Meridian Retail Group (synthetic) is 37.4% of September 2026 revenue and can terminate on sixty days' notice (`documents/02-msa-meridian.pdf` page 2, clause 18.2).
   3. **Rising attrition in delivery roles** — monthly delivery leavers rise from 1 to 4 across the year in `headcount-movements.csv`.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 6 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 192 revenue lines, one per client retainer per month | **Yes** — billing export step |
| `timesheets-summary.csv` | Available and billable hours by team (aggregate) (36 rows) | **Yes** — industry data step |
| `headcount-movements.csv` | Starters, leavers and headcount by role family (aggregate) (24 rows) | **Yes** — industry data step |
| `documents/01-management-pack-2026-09.pdf` | Management pack with reported utilization | **Yes** — documents step |
| `documents/02-msa-meridian.pdf` | Master services agreement with the largest client | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Notes

- People data is aggregate only — no names, no individual records.
