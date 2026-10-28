# Clearbrook Clinics Ltd — Small clinics (GBP)

**Fictional target.** Clearbrook Clinics Ltd runs six dental and physiotherapy clinics with 22 providers, paid by insurers and patients.
Based in Leeds, the United Kingdom; reports in GBP. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Before you start

- Download this whole folder (on GitHub: **Code → Download ZIP** at the top of the repository, then unzip).
- Sign in to Pactlab. The steps take about 15 minutes.
- You upload **4 CSV files** and **2 PDFs**. Nothing else.
- **Never upload the `.md` files** in `documents/`. They are the text each PDF is built from; Pactlab reads the PDFs.
- `vdr-index.csv` is for reference only (how a data room would list these files). Do not upload it.
- Text in **bold** below is a button, tab or option exactly as Pactlab shows it.

## Step 1 — Start the Pact

1. Click **Start a Pact** (top right).
2. **Name the Pact** — Pact name: `Project Clearbrook` · Base currency: **GBP** → **Next**.
3. **Buying entity** — Legal or trading name: `Demo Buyer` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `Clearbrook Clinics Ltd` · **Private** · What kind of company is it?: **Small clinics** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `3200000` (GBP 3,200,000) |
   | Currency | **GBP** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the seller's ask: 1.3× the September 2026 billed revenue run-rate. The demo shows how far the evidence supports it.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `Clearbrook Clinics Ltd`, with the asking price GBP 3,200,000.

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
| 1 | **Upload patient volume** | `patient-volume.csv` | **Upload and map columns** → **Check every row** | **Import 264 rows** |
| 2 | **Upload equipment schedule** | `equipment-schedule.csv` | **Upload and map columns** → **Check every row** | **Import 4 rows** |
| 3 | **Upload coding summary** | `coding-summary.csv` | **Upload and map columns** → **Check every row** | **Import 4 rows** |

**You should see** after each import: "… imported … Industry checks ran on them". Some findings may already appear as drafts; that is expected.

## Step 4 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/01-coding-policy.pdf` | **business information** | Coding and billing policy |
| 2 | `documents/99-data-room-extracts.pdf` | **financial information** | Every CSV extract in this folder as one paged PDF, so findings can cite a page |

**You should see:** all 2 documents listed on the **Documents** tab.

## Step 5 — Run the checks and review the findings

1. Open the **Findings** tab → **Run small clinics checks**.
2. **You should see exactly these 3 findings** (running the checks again adds nothing):

   1. **One provider carries Site 3** — P07 earns 73.8% of Site 3 revenue in `patient-volume.csv` — a retention risk after closing.
   2. **High-complexity coding above policy** — `coding-summary.csv` shows 31–36% of visits at the highest code against the 15% expected by `documents/01-coding-policy.pdf`.
   3. **Imaging equipment past its useful life** — two panoramic X-ray units in `equipment-schedule.csv` (2014 and 2015, ten-year lives). Price as remediation.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 6 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 96 revenue lines, one per payer remittance per month | **Yes** — billing export step |
| `patient-volume.csv` | Visits and revenue by site and pseudonymous provider (264 rows) | **Yes** — industry data step |
| `equipment-schedule.csv` | Equipment with acquisition dates and useful lives (4 rows) | **Yes** — industry data step |
| `coding-summary.csv` | Share of visits billed at the highest complexity code (4 rows) | **Yes** — industry data step |
| `documents/01-coding-policy.pdf` | Coding and billing policy | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Notes

- Providers are pseudonymous (P01, P02, …); Pactlab never sends people data to a model.

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
| `02 Finance/Clearbrook FY26 summary.md` | Pactlab asks: income statement or cash flow statement? | Mixes profit and cash flow lines. |
| `02 Finance/Exports/Clearbrook coding summary export Sep26.csv` | Coding summary |  |
| `02 Finance/Exports/Clearbrook equipment schedule export Sep26.csv` | Equipment schedule |  |
| `02 Finance/Exports/Clearbrook invoice lines export Sep26.csv` | Invoice lines |  |
| `02 Finance/Mgmt accounts FY26 - Clearbrook.md` | Income statement (P&L) | Revenue matches the invoice lines for Oct 2025 – Sep 2026. |
| `05 Policies/Coding policy.pdf` | Policy |  |

**And on the Intake checklist**, these should show as missing: **Cash flow statement**, **Patient volume**.
Once billing is imported, **Customer contract** shows **Some missing** and names the largest billed customers with no contract in the room.
Click **Ask the seller** (or **Copy request for missing items**) to send the list.
