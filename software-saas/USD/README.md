# Brightwave Software Inc. — Software and SaaS (USD)

**Fictional target.** Brightwave Software Inc. sells workflow software to mid-sized logistics and services firms on monthly and annual subscriptions.
Based in Columbus, Ohio, United States; reports in USD. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Before you start

- Download this whole folder (on GitHub: **Code → Download ZIP** at the top of the repository, then unzip).
- Sign in to Pactlab. The steps take about 15 minutes.
- You upload **1 CSV file** and **3 PDFs**. Nothing else.
- **Never upload the `.md` files** in `documents/`. They are the text each PDF is built from; Pactlab reads the PDFs.
- `vdr-index.csv` is for reference only (how a data room would list these files). Do not upload it.
- Text in **bold** below is a button, tab or option exactly as Pactlab shows it.

## Step 1 — Start the Pact

1. Click **Start a Pact** (top right).
2. **Name the Pact** — Pact name: `Project Brightwave` · Base currency: **USD** → **Next**.
3. **Buying entity** — Legal or trading name: `Demo Buyer` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `Brightwave Software Inc.` · **Private** · What kind of company is it?: **Software & SaaS** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `5000000` (USD 5,000,000) |
   | Currency | **USD** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the seller's ask: 8× the September 2026 billed revenue run-rate. The demo shows how far the evidence supports it.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `Brightwave Software Inc.`, with the asking price USD 5,000,000.

## Step 2 — Upload the billing export

1. Open the **Sources** tab → **Upload billing export**.
2. *1. Where is the export from?* → **Pactlab standard template**.
3. *2. Choose the file* → `invoice-lines.csv` → **Upload and map columns**.
4. The columns are matched for you. Click **Check every row**, then **Import 302 lines**.

**You should see:** a green message ending "Finances now include them." The **Finances** tab now shows the revenue ledger.

## Step 3 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/01-board-kpi-pack-2026-09.pdf` | **business information** | Management KPI pack with reported ARR |
| 2 | `documents/02-master-services-agreement-northgate.pdf` | **business information** | Largest customer contract, with change-of-control clause |
| 3 | `documents/03-balance-sheet-2026-09-30.pdf` | **financial information** | Balance sheet with debt and debt-like items |

**You should see:** all 3 documents listed on the **Documents** tab.

## Step 4 — Connect the code and delivery data (Engineering)

Code and delivery data come through their APIs, never as files. Local and dev Pactlab include a synthetic Brightwave repository and Jira site for this:

1. Open the **Sources** tab → **Connect synthetic code and Jira data**.
2. Repository: **brightwave/platform** · Jira site: **brightwave.atlassian.net (BW)** → **Connect and sync**.
3. Pactlab opens **Engineering** when the sync finishes (a few seconds).

**You should see** on **Engineering**: the Brightwave team (six engineers and a product manager who files work but never commits), `billing/` maintained by one person, one engineer marked departed, and delivery slipping in the last two sprints. On **Findings**, two engineering drafts:

- **Single-contributor concentration in billing/** — one engineer wrote every billing change.
- **Commits attributed to unmatched or departed identities** — commits still arrive under an engineer who left in May.

## Step 5 — Run the checks and review the findings

1. Open the **Findings** tab → **Run software & saas checks**.
2. **You should see exactly these 4 findings** (running the checks again adds nothing):

   1. **Management ARR exceeds billed ARR** — the KPI pack reports USD 656,112; `invoice-lines.csv` supports USD 630,312 at September 2026 — a gap of USD 25,800. The KPI pack still counts Quarry Lane Studios, whose last invoice was June 2026.
   2. **Revenue concentration** — Harborline Freight (synthetic) is 27.6% of September 2026 billed revenue.
   3. **Largest customer can leave on a sale** — `documents/02-master-services-agreement-northgate.pdf` page 2, clause 14 — termination on change of control.
   4. **Contraction hidden in the logo count** — Amberline Hotels drops by 30% from April 2026; the KPI pack reports 14 active customers, the ledger has 13.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 6 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 302 revenue lines, one per customer subscription per month | **Yes** — billing export step |
| `documents/01-board-kpi-pack-2026-09.pdf` | Management KPI pack with reported ARR | **Yes** — documents step |
| `documents/02-master-services-agreement-northgate.pdf` | Largest customer contract, with change-of-control clause | **Yes** — documents step |
| `documents/03-balance-sheet-2026-09-30.pdf` | Balance sheet with debt and debt-like items | **Yes** — documents step |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Notes

- Code and delivery data (GitHub, Jira) connect through their APIs, never files. The synthetic Brightwave repository and Jira site in the Engineering step are built into local and dev Pactlab; production connects the real ones.

## Intake test — hand over the whole data room

`dataroom/` is the same material arranged the way a seller hands it over, and `dataroom.zip` is that folder zipped.
Use it to check that Pactlab sorts files on its own and asks only when unsure.

1. Open the pact's **Diligence** tab, then **Documents**.
2. Drop `dataroom.zip` on the upload box and click **Upload**. In local and dev Pactlab you can instead connect the synthetic **Brightwave Software** data room under **Data room**, then **Sync now**.
3. Watch each file get its own row. Clear files are filed with no click from you.
4. Answer the one question under **Pactlab needs you**.

**You should see** each file filed as:

| File in the data room | Pactlab should file it as | Note |
|---|---|---|
| `02 Finance/Board kpi pack 2026 09.pdf` | Other |  |
| `02 Finance/Brightwave FY26 summary.md` | Pactlab asks: income statement or cash flow statement? | Mixes profit and cash flow lines. |
| `02 Finance/Exports/Brightwave invoice lines export Sep26.csv` | Invoice lines |  |
| `02 Finance/Mgmt accounts FY26 - Brightwave.md` | Income statement (P&L) | Revenue matches the invoice lines for Oct 2025 – Sep 2026. |
| `03 Commercial/Customers/Master services agreement northgate (signed copy).pdf` | Duplicate — shown once | Same bytes as the agreement above. |
| `03 Commercial/Customers/Master services agreement northgate.pdf` | Customer contract |  |
| `04 Legal/Balance sheet 2026 09 30.pdf` | Balance sheet | In the Legal folder, but it is a balance sheet: the content decides. |

**And on the Intake checklist**, these should show as missing: **Cash flow statement**.
Once billing is imported, **Customer contract** shows **Some missing** and names the largest billed customers with no contract in the room.
Click **Ask the seller** (or **Copy request for missing items**) to send the list.
