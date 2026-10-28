# Calvera Pharmaceuticals B.V. — Pharma and biotech (EUR)

**Fictional target.** Calvera Pharmaceuticals B.V. is a specialty-pharma company earning royalties and supply revenue on two marketed products, with one late-stage programme.
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
2. **Name the Pact** — Pact name: `Project Calvera` · Base currency: **EUR** → **Next**.
3. **Buying entity** — Legal or trading name: `Demo Buyer` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `Calvera Pharmaceuticals B.V.` · **Private** · What kind of company is it?: **Pharma & biotech** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `36000000` (EUR 36,000,000) |
   | Currency | **EUR** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the seller's ask: 4× the September 2026 billed revenue run-rate. The demo shows how far the evidence supports it.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `Calvera Pharmaceuticals B.V.`, with the asking price EUR 36,000,000.

## Step 2 — Upload the billing export

1. Open the **Sources** tab → **Upload billing export**.
2. *1. Where is the export from?* → **Pactlab standard template**.
3. *2. Choose the file* → `invoice-lines.csv` → **Upload and map columns**.
4. The columns are matched for you. Click **Check every row**, then **Import 96 lines**.

**You should see:** a green message ending "Finances now include them." The **Finances** tab now shows the revenue ledger.

## Step 3 — Upload the industry data

Open the **Sources** tab and scroll to **Industry data**. Upload these files one at a time:

| # | Click | Choose the file | Then | Button should read |
|---|---|---|---|---|
| 1 | **Upload patent schedule** | `patent-schedule.csv` | **Upload and map columns** → **Check every row** | **Import 4 rows** |
| 2 | **Upload pipeline** | `pipeline.csv` | **Upload and map columns** → **Check every row** | **Import 2 rows** |

**You should see** after each import: "… imported … Industry checks ran on them". Some findings may already appear as drafts; that is expected.

## Step 4 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/01-revenue-forecast.pdf` | **business information** | Management revenue forecast and its exclusivity assumption |
| 2 | `documents/02-supplier-inspection-report.pdf` | **business information** | Contract manufacturer inspection summary |
| 3 | `documents/99-data-room-extracts.pdf` | **financial information** | Every CSV extract in this folder as one paged PDF, so findings can cite a page |

**You should see:** all 3 documents listed on the **Documents** tab.

## Step 5 — Run the checks and review the findings

1. Open the **Findings** tab → **Run pharma & biotech checks**.
2. **You should see exactly these 3 findings** (running the checks again adds nothing):

   1. **Key patent expires earlier than the forecast assumes** — the forecast assumes exclusivity through 2031; `patent-schedule.csv` shows the Product A composition-of-matter patents expiring in 2028.
   2. **Open manufacturing observations at the supplier** — `documents/02-supplier-inspection-report.pdf` page 2 — three open observations.
   3. **Partner concentration** — Aldermoor Therapeutics accounts for both of the two largest revenue lines; the royalty line alone is 59.1% of September 2026 revenue.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 6 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 96 revenue lines, one per partner royalty and supply payment per month | **Yes** — billing export step |
| `patent-schedule.csv` | Patent families, products and expiry dates (4 rows) | **Yes** — industry data step |
| `pipeline.csv` | Development pipeline and next milestones (2 rows) | **Yes** — industry data step |
| `documents/01-revenue-forecast.pdf` | Management revenue forecast and its exclusivity assumption | **Yes** — documents step |
| `documents/02-supplier-inspection-report.pdf` | Contract manufacturer inspection summary | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Intake test — hand over the whole data room

`dataroom/` is the same material arranged the way a seller hands it over, and `dataroom.zip` is that folder zipped.
Use it to check that Pactlab sorts files on its own and asks only when unsure.

1. Open the pact's **Diligence** tab, then **Documents**.
2. Drop `dataroom.zip` on the upload box and click **Upload**.
3. Watch each file get its own row. Clear files are filed with no click from you.
4. Answer the one question under **Pactlab needs you**.

**You should see** each file filed as:

| File in the data room | Pactlab should file it as | Note |
|---|---|---|
| `02 Finance/Calvera FY26 summary.md` | Pactlab asks: income statement or cash flow statement? | Mixes profit and cash flow lines. |
| `02 Finance/Exports/Calvera invoice lines export Sep26.csv` | Invoice lines |  |
| `02 Finance/Exports/Calvera patent schedule export Sep26.csv` | Patent schedule |  |
| `02 Finance/Mgmt accounts FY26 - Calvera.md` | Income statement (P&L) | Revenue matches the invoice lines for Oct 2025 – Sep 2026. |
| `02 Finance/Revenue forecast.pdf` | Other |  |
| `03 Commercial/Suppliers/Supplier inspection report.pdf` | Supplier contract |  |

**And on the Intake checklist**, these should show as missing: **Cash flow statement**, **Pipeline**.
Once billing is imported, **Customer contract** shows **Some missing** and names the largest billed customers with no contract in the room.
Click **Ask the seller** (or **Copy request for missing items**) to send the list.
