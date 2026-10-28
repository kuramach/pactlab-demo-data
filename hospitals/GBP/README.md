# St. Brennan Health Ltd — Hospitals (GBP)

**Fictional target.** St. Brennan Health Ltd operates St. Brennan Regional Medical Center, a 220-bed acute-care hospital with cardiology, orthopaedics and maternity service lines.
Based in Leeds, the United Kingdom; reports in GBP. Data runs October 2024 to September 2026.

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
2. **Name the Pact** — Pact name: `Project St.` · Base currency: **GBP** → **Next**.
3. **Buying entity** — Legal or trading name: `Demo Buyer` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `St. Brennan Health Ltd` · **Private** · What kind of company is it?: **Hospitals** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `33000000` (GBP 33,000,000) |
   | Currency | **GBP** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the seller's ask: 1× the September 2026 billed revenue run-rate. The demo shows how far the evidence supports it.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `St. Brennan Health Ltd`, with the asking price GBP 33,000,000.

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
| 1 | **Upload census** | `census.csv` | **Upload and map columns** → **Check every row** | **Import 48 rows** |
| 2 | **Upload payer mix** | `payer-mix.csv` | **Upload and map columns** → **Check every row** | **Import 60 rows** |

**You should see** after each import: "… imported … Industry checks ran on them". Some findings may already appear as drafts; that is expected.

## Step 4 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/01-accreditation-record.pdf` | **business information** | Accreditation record and transfer condition |
| 2 | `documents/02-medicare-cost-report-summary.pdf` | **financial information** | Cost report summary with committed regulatory capex |
| 3 | `documents/03-service-line-dependence.pdf` | **business information** | Aggregate physician dependence by service line |
| 4 | `documents/99-data-room-extracts.pdf` | **financial information** | Every CSV extract in this folder as one paged PDF, so findings can cite a page |

**You should see:** all 4 documents listed on the **Documents** tab.

## Step 5 — Run the checks and review the findings

1. Open the **Findings** tab → **Run hospitals checks**.
2. **You should see exactly these 4 findings** (running the checks again adds nothing):

   1. **Earnings concentrated in one payer** — Government programme A (synthetic) is 56.3% of September 2026 net revenue.
   2. **Accreditation does not transfer automatically** — `documents/01-accreditation-record.pdf` page 2 — make it a closing condition.
   3. **Key-physician dependence in cardiology** — `documents/03-service-line-dependence.pdf` — two physicians perform about 80% of cardiology procedures (aggregate data only).
   4. **Committed regulatory capex** — `documents/02-medicare-cost-report-summary.pdf` — GBP 3,239,000 committed. Price as remediation.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 6 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 120 revenue lines, one per payer net-revenue settlement per month | **Yes** — billing export step |
| `census.csv` | Admissions and census by service line (48 rows) | **Yes** — industry data step |
| `payer-mix.csv` | Gross charges and net revenue by payer (60 rows) | **Yes** — industry data step |
| `documents/01-accreditation-record.pdf` | Accreditation record and transfer condition | **Yes** — documents step |
| `documents/02-medicare-cost-report-summary.pdf` | Cost report summary with committed regulatory capex | **Yes** — documents step |
| `documents/03-service-line-dependence.pdf` | Aggregate physician dependence by service line | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Notes

- Physician data is aggregate only; Pactlab never sends people data to a model.

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
| `02 Finance/Exports/St. census export Sep26.csv` | Census |  |
| `02 Finance/Exports/St. invoice lines export Sep26.csv` | Invoice lines |  |
| `02 Finance/Medicare cost report summary.pdf` | Other |  |
| `02 Finance/Mgmt accounts FY26 - St..md` | Income statement (P&L) | Revenue matches the invoice lines for Oct 2025 – Sep 2026. |
| `02 Finance/Service line dependence.pdf` | Other |  |
| `02 Finance/St. FY26 summary.md` | Pactlab asks: income statement or cash flow statement? | Mixes profit and cash flow lines. |
| `04 Legal/Accreditation record.pdf` | Loan agreement |  |

**And on the Intake checklist**, these should show as missing: **Cash flow statement**, **Payer mix**.
Once billing is imported, **Customer contract** shows **Some missing** and names the largest billed customers with no contract in the room.
Click **Ask the seller** (or **Copy request for missing items**) to send the list.
