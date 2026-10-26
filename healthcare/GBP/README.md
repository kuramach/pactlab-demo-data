# Riverside Care Partners Ltd — Healthcare services and healthtech (GBP)

**Fictional target.** Riverside Care Partners Ltd operates nine physical-therapy and primary-care practices, paid mostly by government programmes and commercial insurers.
Based in Leeds, the United Kingdom; reports in GBP. Data runs October 2024 to September 2026.

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
2. **Name the Pact** — Pact name: `Project Riverside` · Base currency: **GBP** → **Next**.
3. **Buying entity** — Legal or trading name: `Demo Buyer` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `Riverside Care Partners Ltd` · **Private** · What kind of company is it?: **Healthcare & health tech** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `1900000` (GBP 1,900,000) |
   | Currency | **GBP** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the seller's ask: 1.5× the September 2026 billed revenue run-rate. The demo shows how far the evidence supports it.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `Riverside Care Partners Ltd`, with the asking price GBP 1,900,000.

## Step 2 — Upload the billing export

1. Open the **Sources** tab → **Upload billing export**.
2. *1. Where is the export from?* → **Pactlab standard template**.
3. *2. Choose the file* → `invoice-lines.csv` → **Upload and map columns**.
4. The columns are matched for you. Click **Check every row**, then **Import 144 lines**.

**You should see:** a green message ending "Finances now include them." The **Finances** tab now shows the revenue ledger.

## Step 3 — Upload the industry data

Open the **Sources** tab and scroll to **Industry data**. Upload these files one at a time:

| # | Click | Choose the file | Then | Button should read |
|---|---|---|---|---|
| 1 | **Upload claims summary** | `claims-summary.csv` | **Upload and map columns** → **Check every row** | **Import 72 rows** |
| 2 | **Upload provider roster** | `provider-roster.csv` | **Upload and map columns** → **Check every row** | **Import 18 rows** |

**You should see** after each import: "… imported … Industry checks ran on them". Some findings may already appear as drafts; that is expected.

## Step 4 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/01-medical-director-agreement.pdf` | **business information** | Medical-director agreement and time records |
| 2 | `documents/02-privacy-risk-assessment.pdf` | **business information** | Most recent privacy and security risk assessment |
| 3 | `documents/99-data-room-extracts.pdf` | **financial information** | Every CSV extract in this folder as one paged PDF, so findings can cite a page |

**You should see:** all 3 documents listed on the **Documents** tab.

## Step 5 — Run the checks and review the findings

1. Open the **Findings** tab → **Run healthcare & health tech checks**.
2. **You should see exactly these 4 findings** (running the checks again adds nothing):

   1. **Revenue concentrated in government programmes** — government programmes A and B are 63.4% of September 2026 revenue in `invoice-lines.csv`.
   2. **Medical-director fee above documented duties** — `documents/01-medical-director-agreement.pdf` — a fixed fee for four hours a month, against 1.5 documented hours (page 2).
   3. **Privacy risk assessment out of date** — `documents/02-privacy-risk-assessment.pdf` — last assessed March 2023, review overdue since March 2024.
   4. **Provider credentials expiring** — two providers in `provider-roster.csv` have credentials expiring before the end of 2026.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 6 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 144 revenue lines, one per payer remittance per month | **Yes** — billing export step |
| `claims-summary.csv` | Monthly claims billed, paid and denial rate by payer (72 rows) | **Yes** — industry data step |
| `provider-roster.csv` | Provider roster, pseudonymous, with credential expiry dates (18 rows) | **Yes** — industry data step |
| `documents/01-medical-director-agreement.pdf` | Medical-director agreement and time records | **Yes** — documents step |
| `documents/02-privacy-risk-assessment.pdf` | Most recent privacy and security risk assessment | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Notes

- Provider data is pseudonymous and aggregate by design; Pactlab never sends people data to a model.
