# Larkfield Residential Ltd — Multifamily (GBP)

**Fictional target.** Larkfield Residential Ltd owns Larkfield Commons, a 96-unit garden-style apartment community in three buildings (A, B, C).
Based in Leeds, the United Kingdom; reports in GBP. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Before you start

- Download this whole folder (on GitHub: **Code → Download ZIP** at the top of the repository, then unzip).
- Sign in to Pactlab. The steps take about 15 minutes.
- You upload **5 CSV files** and **2 PDFs**. Nothing else.
- **Never upload the `.md` files** in `documents/`. They are the text each PDF is built from; Pactlab reads the PDFs.
- `vdr-index.csv` is for reference only (how a data room would list these files). Do not upload it.
- Text in **bold** below is a button, tab or option exactly as Pactlab shows it.

## Step 1 — Start the Pact

1. Click **Start a Pact** (top right).
2. **Name the Pact** — Pact name: `Project Larkfield` · Base currency: **GBP** → **Next**.
3. **Buying entity** — Legal or trading name: `Demo Buyer` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `Larkfield Residential Ltd` · **Private** · What kind of company is it?: **Multifamily** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `17000000` (GBP 17,000,000) |
   | Currency | **GBP** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the seller's ask: 12× the September 2026 billed revenue run-rate. The demo shows how far the evidence supports it.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `Larkfield Residential Ltd`, with the asking price GBP 17,000,000.

## Step 2 — Upload the billing export

1. Open the **Sources** tab → **Upload billing export**.
2. *1. Where is the export from?* → **Pactlab standard template**.
3. *2. Choose the file* → `invoice-lines.csv` → **Upload and map columns**.
4. The columns are matched for you. Click **Check every row**, then **Import 2160 lines**.

**You should see:** a green message ending "Finances now include them." The **Finances** tab now shows the revenue ledger.

## Step 3 — Upload the industry data

Open the **Sources** tab and scroll to **Industry data**. Upload these files one at a time:

| # | Click | Choose the file | Then | Button should read |
|---|---|---|---|---|
| 1 | **Upload rent roll** | `rent-roll.csv` | **Upload and map columns** → **Check every row** | **Import 96 rows** |
| 2 | **Upload t-12 operating statement** | `t12.csv` | **Upload and map columns** → **Check every row** | **Import 12 rows** |
| 3 | **Upload delinquency report** | `delinquency.csv` | **Upload and map columns** → **Check every row** | **Import 7 rows** |
| 4 | **Upload unit inspections** | `unit-inspections.csv` | **Upload and map columns** → **Check every row** | **Import 96 rows** |

**You should see** after each import: "… imported … Industry checks ran on them". Some findings may already appear as drafts; that is expected.

## Step 4 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/01-offering-memorandum.pdf` | **business information** | Offering memorandum with stated NOI and capital plan |
| 2 | `documents/99-data-room-extracts.pdf` | **financial information** | Every CSV extract in this folder as one paged PDF, so findings can cite a page |

**You should see:** all 2 documents listed on the **Documents** tab.

## Step 5 — Run the checks and review the findings

1. Open the **Findings** tab → **Run multifamily checks**.
2. **You should see exactly these 4 findings** (running the checks again adds nothing):

   1. **Offering memorandum NOI above the T-12** — the memorandum states GBP 947,320; `t12.csv` sums to GBP 853,441 — the memorandum uses pro-forma rents.
   2. **Deferred maintenance above the capital plan** — `unit-inspections.csv` estimates GBP 145,834 of repairs against a GBP 113,760 capital plan — GBP 1,519 per door. Price as remediation.
   3. **Delinquency concentrated in Building C** — 85.7% of delinquent units in `delinquency.csv` are in Building C.
   4. **Loss-to-lease (upside, not price)** — occupied units are 7.7% below market rent in `rent-roll.csv`. Record it as confirmed value — never as a reason to pay more.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 6 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 2160 revenue lines, one per unit rent charge per month | **Yes** — billing export step |
| `rent-roll.csv` | Rent roll at 30 September 2026 (96 rows) | **Yes** — industry data step |
| `delinquency.csv` | Delinquent balances at 30 September 2026 (7 rows) | **Yes** — industry data step |
| `unit-inspections.csv` | Unit-condition inspections with repair estimates (96 rows) | **Yes** — industry data step |
| `t12.csv` | Trailing-twelve-month operating statement (T-12) (12 rows) | **Yes** — industry data step |
| `documents/01-offering-memorandum.pdf` | Offering memorandum with stated NOI and capital plan | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Notes

- Residents are referred to by unit only; there are no personal names.
- The rent roll maps onto the billing import: each occupied unit is a customer billed monthly.
