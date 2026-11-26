# St. Brennan Health Inc. — Hospitals (USD)

**Fictional target.** St. Brennan Health Inc. operates St. Brennan Regional Medical Center, a 220-bed acute-care hospital with cardiology, orthopaedics and maternity service lines.
Based in Columbus, Ohio, United States; reports in USD. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Before you start

- Download this whole folder (on GitHub: **Code → Download ZIP** at the top of the repository, then unzip).
- Sign in to Pactlab. The steps take about 15 minutes.
- You upload **4 CSV files** and **9 PDFs**. Nothing else.
- **Never upload the `.md` files** in `documents/`. They are the text each PDF is built from; Pactlab reads the PDFs.
- `vdr-index.csv` is for reference only (how a data room would list these files). Do not upload it.
- Text in **bold** below is a button, tab or option exactly as Pactlab shows it.

## Two ways to test this company

- **Part A — Buyer side** (Steps 1 onwards): you are a buyer doing diligence on St. Brennan Health Inc..
- **Part B — Seller side** ([below](#part-b--seller-side-run-a-bid-process)): you are St. Brennan Health Inc., inviting several buyers — they ask questions, then offer or pass, and you choose one. Uses `bidders.csv`.
- Each part starts its own Pact, so you can do either one, or both.

# Part A — Buyer side

## Step 1 — Start the Pact

1. Click **Start a Pact** (top right).
2. **Name the Pact** — Pact name: `Project St.` · Base currency: **USD** → **Next**.
3. **Buying entity** — Legal or trading name: `Demo Buyer` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `St. Brennan Health Inc.` · **Private** · What kind of company is it?: **Hospitals** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `42000000` (USD 42,000,000) |
   | Currency | **USD** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the seller's ask: 1× the September 2026 billed revenue run-rate. The demo shows how far the evidence supports it.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `St. Brennan Health Inc.`, with the asking price USD 42,000,000.

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
| 3 | **Upload medical-staff register** | `medical-staff.csv` | **Upload and map columns** → **Check every row** | **Import 55 rows** |

**You should see** after each import: "… imported … Industry checks ran on them". Some findings may already appear as drafts; that is expected.

## Step 4 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/01-accreditation-record.pdf` | **business information** | Accreditation record and transfer condition |
| 2 | `documents/02-medicare-cost-report-summary.pdf` | **financial information** | Filed cost report summary: beds, inpatient days, occupancy, payer shares, costs and committed regulatory capex |
| 3 | `documents/03-service-line-dependence.pdf` | **business information** | Aggregate physician dependence by service line |
| 4 | `documents/04-management-presentation.pdf` | **business information** | Management presentation: occupancy, payer mix, plant, quality rating and the target closing date |
| 5 | `documents/05-payer-agreement-keystone.pdf` | **business information** | Payer agreement with Commercial plan Keystone: rate basis, term and renewal |
| 6 | `documents/06-payer-agreement-riverbend.pdf` | **business information** | Payer agreement with Commercial plan Riverbend: rate basis, term and renewal |
| 7 | `documents/07-property-condition-assessment.pdf` | **business information** | Property condition assessment of the hospital plant |
| 8 | `documents/08-quality-reporting.pdf` | **business information** | Published quality reporting: the overall star rating |
| 9 | `documents/99-data-room-extracts.pdf` | **financial information** | Every CSV extract in this folder as one paged PDF, so findings can cite a page |

**You should see:** all 9 documents listed on the **Documents** tab.

## Step 5 — Upload the P&L by year

Open the **Sources** tab, scroll to **Industry data** and click **Upload profit and loss (p&l)**.

1. Choose `pnl.csv` → **Upload and map columns**. Pactlab reads the three years across the columns (FY2023, FY2024, FY2025).
2. Say what each line is: the two lines ending in *revenue* are **Revenue**, `Cost of care: staff salaries and benefits` is **Cost of revenue**, and the rest are **Operating expenses**.
3. **Check every row**, then **Import 27 rows**.

**You should see:** the import succeed. The **Hospital** tab shows capital spend year by year, and the checks in the next step read every year.

## Step 6 — Run the checks and review the findings

1. Open the **Findings** tab → **Run hospitals checks**.
2. **You should see exactly these 11 findings** (running the checks again adds nothing):

   1. **Earnings concentrated in one payer** — Government programme A (synthetic) is 56.7% of September 2026 net revenue.
   2. **Accreditation does not transfer automatically** — `documents/01-accreditation-record.pdf` page 2 — make it a closing condition.
   3. **Key-physician dependence in cardiology** — `documents/03-service-line-dependence.pdf` — two physicians perform about 80% of cardiology procedures (aggregate data only).
   4. **Committed regulatory capex** — `documents/02-medicare-cost-report-summary.pdf` — USD 4,100,000 committed. Price as remediation.
   5. **The cost report contradicts the deck: Occupancy of licensed beds** — `documents/04-management-presentation.pdf` says 82%; the filed cost report for fiscal year 2025 says 66.4% (`documents/02-medicare-cost-report-summary.pdf`).
   6. **Claim verified against the cost report: Medicare share of inpatient days** — 41% in the deck, 41.0% in the cost report.
   7. **Largest payer contract ends 7 months after closing: Commercial plan Keystone (synthetic)** — `documents/05-payer-agreement-keystone.pdf` — the term ends on 31 July 2027, seven months after the 31 December 2026 target closing in the deck; Keystone is the largest contracted payer in `payer-mix.csv`.
   8. **Orthopaedics: clinical privileges lapsed together for 7 medical staff on 2026-06-30** — `medical-staff.csv` — all 7 orthopaedic surgeons share the 30 June 2026 reappointment date, passed with no reappointment recorded.
   9. **Capital spend fell from 6.1% to 2.6% of revenue, 2023–2025, against a “modern plant” claim** — `pnl.csv` — capital-related costs fall every year (USD 2,135,000 to USD 1,024,400) while the deck claims a modern plant; `documents/07-property-condition-assessment.pdf` puts deferred maintenance at USD 6,800,000. One year alone misses it.
   10. **Quality claim verified: overall star rating** — four stars in the deck, 4 stars in `documents/08-quality-reporting.pdf` — the stated rating only.
   11. **P&L trend, 2023–2025** — every imported year side by side: revenue, growth, margins and the labour, contract labour, supplies, capital and repairs ratios.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 7 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

# Part B — Seller side: run a bid process

Here you are St. Brennan Health Inc. You invite three bidders from `bidders.csv`, share a little, answer their questions and choose one.
Each bidder sees only their own bid — never another bidder's questions, offers or whether they passed. Part B checks that too.

**Addresses.** This folder holds no email addresses. Invite **an address you can read for each firm**: your own address with `+` and the firm's tag from `bidders.csv` added before the @ (for tag `harbor`: *yourname+harbor* at your email domain — Gmail, Outlook and most providers deliver it to you). On your own computer (`pnpm dev`) any made-up address works: every email Pactlab sends, invitations and sign-in codes, is written to `apps/api/.data/mail/`.

## Step B1 — Start the Pact as the seller

1. Click **Start a Pact** (top right).
2. Under *Who are you in this deal?* choose **We are selling (or raising)**. Pact name: `Project St. Sale` · Base currency: **USD** → **Next**. (There is no buying-entity step.)
3. **Selling entity** — Legal or trading name: `St. Brennan Health Inc.` · **Private** · What kind of company is it?: **Hospitals** → **Next**.
4. **Asking price** — enter the same asking price as Part A, Step 1 (`42000000`) → **Next**.
5. **Review and start** — the Buyer box says *Bid process — you invite buyers once the pact starts* → **Start Pact**.

**You should see:** the **Bidders** page, with no bidders yet.

## Step B2 — Decide what bidders see

On **Bidders**, under **What bidders see**:

| Field | Enter |
|---|---|
| Shared summary | `St. Brennan Health Inc. operates St. Brennan Regional Medical Center, a 220-bed acute-care hospital with cardiology, orthopaedics and maternity service lines.` |
| Your data room (link) | `https://dataroom.example/hospitals` (Pactlab is not the data room; this is where you would grant access) |
| NDA | `Mutual NDA (synthetic): everything shared about St. Brennan Health Inc. stays confidential.` |
| Offer deadline (UTC) | a date a week from today |

→ **Save**.

Then open the **Documents** tab and upload `documents/01-accreditation-record.pdf` with **Share with bidders** ticked (it is chosen at upload and cannot be changed later). Upload nothing else as shared — the rest stays with you.

**You should see:** "Saved. Bidders see the shared view once they accept the NDA." On Documents, `01-accreditation-record.pdf` is listed.

## Step B3 — Add the three bidders and invite them

On **Bidders**, for each row of `bidders.csv`:

| Bidding firm | Then invite | Tag |
|---|---|---|
| `Harbor Capital Partners (synthetic)` → **Add bidder** | your address with `+harbor` in *Invite someone from Harbor Capital Partners (synthetic)* → **Invite** | `harbor` |
| `Northline Strategic (synthetic)` → **Add bidder** | your address with `+northline` in *Invite someone from Northline Strategic (synthetic)* → **Invite** | `northline` |
| `Atlas Growth Equity (synthetic)` → **Add bidder** | your address with `+atlas` in *Invite someone from Atlas Growth Equity (synthetic)* → **Invite** | `atlas` |

**You should see:** three firms marked **Invited**, each listing the address you invited.

## Step B4 — Be each bidder (a private window per bidder)

For each bidder: open the invitation link (from the email, or the newest file in `apps/api/.data/mail/`) in a **private window**, create the account with the firm's name, sign in with the code, then **Accept and open the pact**.

1. You land on **Your bid** and see only the NDA. Click **I accept the NDA** — the shared summary, the data-room link and the shared document appear.
2. **Harbor Capital Partners (synthetic)**: ask `Can any customer or supplier contract be ended on a change of control?` → **Ask**. Then offer:

   | Field | Enter |
   |---|---|
   | Price | `39000000` (USD 39,000,000) |
   | Currency | `USD` |
   | Structure (cash, shares, earn-out…) | `Cash at close for 100% of the shares` |
   | Conditions | `Subject to confirmatory diligence and committed financing` |

   → **Submit offer**.
3. **Northline Strategic (synthetic)**: ask `Can you share the last three years of audited accounts?` → **Ask**. Then offer **Price** `36000000` (USD 36,000,000), **Structure** `80% cash at close, 20% earn-out over 24 months`, **Conditions** `Key-person retention for the founders` → **Submit offer**.
4. **Atlas Growth Equity (synthetic)**: accept the NDA, then type `Outside our sector focus this year.` as the reason → **Pass on this pact**.

**You should see**, as Northline Strategic (synthetic): your own question and offer only — nothing of Harbor Capital Partners (synthetic)'s question or offer, and no sign that Atlas Growth Equity (synthetic) passed. There are no deal tabs; trying `/deals/<id>/bidders` shows nothing of the seller's side.

## Step B5 — Answer the questions

Back as the seller (your normal window), on **Bidders** under **Questions from bidders**:

- Harbor Capital Partners (synthetic)'s question → answer `One customer contract has a change-of-control clause; it is in the shared documents.` → choose **All bidders (without naming who asked)** → **Answer**.
- Northline Strategic (synthetic)'s question → answer `FY2024 and FY2025 are audited; FY2026 closes in December. We will add them to the data room.` → keep **Only Northline Strategic (synthetic)** → **Answer**.

**You should see**, as Northline Strategic (synthetic) (refresh **Your bid**): your private answer, and under *Answered to all bidders* the change-of-control question — without the name of who asked it. Harbor Capital Partners (synthetic) sees the answer to all, but not Northline Strategic (synthetic)'s private one.

## Step B6 — Compare the offers

On **Bidders**, **Offers side by side** sets the two offers next to each other — price, structure, conditions, version. Pactlab does not rank them or recommend one.

**You should see:** Harbor Capital Partners (synthetic) at USD 39,000,000 and Northline Strategic (synthetic) at USD 36,000,000; Atlas Growth Equity (synthetic) marked **Passed** with its reason.

## Step B7 — Shortlist, run round 2 and choose

1. Click **Shortlist** on Harbor Capital Partners (synthetic) and on Northline Strategic (synthetic), then **Start round 2 with 2 shortlisted**.
2. As each bidder, submit a revised offer on **Your bid**: Harbor Capital Partners (synthetic) `41000000`, Northline Strategic (synthetic) `37000000` → **Submit revised offer**. Every version stays listed.
3. As the seller, click **Award to Harbor Capital Partners (synthetic)**.

**You should see:** "Awarded. Every other bidder has been declined and their access ended." Harbor Capital Partners (synthetic)'s **Your bid** says **Selected by the seller**; Northline Strategic (synthetic) can no longer open the pact. The **Team** tab and the audit log record every step.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 120 revenue lines, one per payer net-revenue settlement per month | **Yes** — billing export step |
| `census.csv` | Admissions and census by service line (48 rows) | **Yes** — industry data step |
| `payer-mix.csv` | Gross charges and net revenue by payer (60 rows) | **Yes** — industry data step |
| `medical-staff.csv` | Medical-staff register: department, licence and clinical privileges by pseudonymous staff reference (55 rows) | **Yes** — industry data step |
| `pnl.csv` | Profit and loss by fiscal year, FY2023 to FY2025 (9 lines) | **Yes** — P&L step |
| `documents/01-accreditation-record.pdf` | Accreditation record and transfer condition | **Yes** — documents step |
| `documents/02-medicare-cost-report-summary.pdf` | Filed cost report summary: beds, inpatient days, occupancy, payer shares, costs and committed regulatory capex | **Yes** — documents step |
| `documents/03-service-line-dependence.pdf` | Aggregate physician dependence by service line | **Yes** — documents step |
| `documents/04-management-presentation.pdf` | Management presentation: occupancy, payer mix, plant, quality rating and the target closing date | **Yes** — documents step |
| `documents/05-payer-agreement-keystone.pdf` | Payer agreement with Commercial plan Keystone: rate basis, term and renewal | **Yes** — documents step |
| `documents/06-payer-agreement-riverbend.pdf` | Payer agreement with Commercial plan Riverbend: rate basis, term and renewal | **Yes** — documents step |
| `documents/07-property-condition-assessment.pdf` | Property condition assessment of the hospital plant | **Yes** — documents step |
| `documents/08-quality-reporting.pdf` | Published quality reporting: the overall star rating | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `bidders.csv` | The three bidding firms for Part B: who to invite, what each asks and offers | **No** — read it while you follow Part B |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Notes

- Physician data is aggregate only; the medical-staff register names staff by pseudonymous reference (MS-001, …). Pactlab never sends people data to a model.
- The P&L (`pnl.csv`) imports through Sources like any extract; the multi-year checks read every year it holds. A single year still imports: the trend then reports that year alone.
- Diligence support only: the pack reconciles documents, dates and arithmetic. It does not predict a survey outcome, assess the quality of care or read a contract in law.

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
| `02 Finance/Management presentation.pdf` | Other |  |
| `02 Finance/Medicare cost report summary.pdf` | Other |  |
| `02 Finance/Mgmt accounts FY26 - St..md` | Income statement (P&L) | Revenue matches the invoice lines for Oct 2025 – Sep 2026. |
| `02 Finance/Property condition assessment.pdf` | Other |  |
| `02 Finance/Quality reporting.pdf` | Other |  |
| `02 Finance/Service line dependence.pdf` | Other |  |
| `02 Finance/St. FY26 summary.md` | Pactlab asks: income statement or cash flow statement? | Mixes profit and cash flow lines. |
| `03 Commercial/Customers/Payer agreement keystone (signed copy).pdf` | Duplicate — shown once | Same bytes as the agreement above. |
| `03 Commercial/Customers/Payer agreement keystone.pdf` | Customer contract |  |
| `03 Commercial/Customers/Payer agreement riverbend.pdf` | Customer contract |  |
| `04 Legal/Accreditation record.pdf` | Loan agreement |  |

**And on the Intake checklist**, these should show as missing: **Cash flow statement**, **Payer mix**.
Once billing is imported, **Customer contract** shows **Some missing** and names the largest billed customers with no contract in the room.
Click **Ask the seller** (or **Copy request for missing items**) to send the list.
