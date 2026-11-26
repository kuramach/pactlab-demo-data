# St. Brennan Health Inc. — Hospitals (USD)

**Fictional target.** St. Brennan Health Inc. operates St. Brennan Regional Medical Center, a 220-bed acute-care hospital with cardiology, orthopaedics and maternity service lines.
Based in Columbus, Ohio, United States; reports in USD. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Before you start

- Download this whole folder (on GitHub: **Code → Download ZIP** at the top of the repository, then unzip).
- Sign in to Pactlab. The steps take about 15 minutes.
- You upload **6 CSV files** and **10 PDFs**. Nothing else.
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
| 3 | **Upload medical-staff roster** | `medical-staff.csv` | **Upload and map columns** → **Check every row** | **Import 56 rows** |
| 4 | **Upload capital spend history** | `capex-history.csv` | **Upload and map columns** → **Check every row** | **Import 9 rows** |

**You should see** after each import: "… imported … Industry checks ran on them". Some findings may already appear as drafts; that is expected.

## Step 4 — Upload the P&L, by year

`pnl.csv` holds the profit and loss for fiscal years 2024, 2025, 2026, one column per year. Pactlab reads every year, so the trend across them shows.

1. On **Sources**, under **Industry data**, click **Upload profit and loss (p&l)** → `pnl.csv` → **Upload and map columns**.
2. The line names and the years are read from the file. Under **What each line is**, choose:

   | Line | What it is |
   |---|---|
   | `Net patient service revenue` | **Revenue** |
   | `Other operating revenue` | **Revenue** |
   | `Salaries and benefits` | **Operating expense** |
   | `Contract labour` | **Operating expense** |
   | `Medical supplies and drugs` | **Cost of revenue** |
   | `Purchased services` | **Operating expense** |
   | `Utilities and occupancy` | **Operating expense** |
   | `Other operating expenses` | **Operating expense** |

3. Click **Check every row**, then **Import 24 rows**.

**You should see:** the statement for each year, adding up. **Quality of earnings** and **Valuation** read every imported year.

## Step 5 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/01-accreditation-record.pdf` | **business information** | Accreditation record and transfer condition |
| 2 | `documents/02-medicare-cost-report-summary.pdf` | **financial information** | Filed cost report summary: days, costs and committed regulatory capex |
| 3 | `documents/03-service-line-dependence.pdf` | **business information** | Aggregate physician dependence by service line |
| 4 | `documents/04-management-presentation.pdf` | **business information** | The seller's management presentation (the deck) |
| 5 | `documents/05-quality-reporting-summary.pdf` | **business information** | Published quality-reporting summary |
| 6 | `documents/06-property-condition-assessment.pdf` | **business information** | Property condition assessment of the hospital plant |
| 7 | `documents/07-payer-agreement-keystone.pdf` | **business information** | Payer agreement: Commercial plan Keystone |
| 8 | `documents/08-payer-agreement-riverbend.pdf` | **business information** | Payer agreement: Commercial plan Riverbend |
| 9 | `documents/09-transaction-timetable.pdf` | **business information** | Transaction timetable |
| 10 | `documents/99-data-room-extracts.pdf` | **financial information** | Every CSV extract in this folder as one paged PDF, so findings can cite a page |

**You should see:** all 10 documents listed on the **Documents** tab.

## Step 6 — Run the checks and review the findings

1. Open the **Findings** tab → **Run hospitals checks**.
2. **You should see exactly these 9 findings** (running the checks again adds nothing):

   1. **Earnings concentrated in one payer** — Government programme A (synthetic) is 56.7% of September 2026 net revenue.
   2. **Accreditation does not transfer automatically** — `documents/01-accreditation-record.pdf` page 2 — make it a closing condition.
   3. **Key-physician dependence in cardiology** — `documents/03-service-line-dependence.pdf` — two physicians perform about 80% of cardiology procedures (aggregate data only).
   4. **Committed regulatory capex** — `documents/02-medicare-cost-report-summary.pdf` — USD 4,100,000 committed. Price as remediation.
   5. **Largest payer contract expires 7 months after closing** — `documents/07-payer-agreement-keystone.pdf` ends 31 August 2027, seven months after the target closing date in `documents/09-transaction-timetable.pdf`; Keystone is 18.6% of net revenue in `payer-mix.csv`.
   6. **Cost-report occupancy contradicts the deck** — `documents/02-medicare-cost-report-summary.pdf` gives 54,020 inpatient days of 80,300 available (67.3%); `documents/04-management-presentation.pdf` claims 82%.
   7. **Capex falling against a modern-plant claim** — `capex-history.csv` over `pnl.csv` revenue: 7.0%, 4.9%, 2.8% of revenue over 2024–2026, while the deck claims a modern plant and `documents/06-property-condition-assessment.pdf` lists USD 6,800,000 of deferred maintenance. Any one year looks ordinary.
   8. **Orthopaedics privileges lapsed together on 2026-08-31** — `medical-staff.csv` — six of the seven orthopaedic surgeons share one privilege-renewal date, already passed when the data ends (2026-09-30). A closing condition.
   9. **Published star rating verified** — the deck's 4-star claim matches `documents/05-quality-reporting-summary.pdf` (confirmed value, never a price increase).

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
| `medical-staff.csv` | Medical-staff roster: pseudonymous physicians, licence and privilege dates (56 rows) | **Yes** — industry data step |
| `capex-history.csv` | Capital spend by fiscal year and category (9 rows) | **Yes** — industry data step |
| `pnl.csv` | Profit and loss by fiscal year (8 lines × 3 years) | **Yes** — P&L step |
| `pnl-line-kinds.csv` | What each P&L line is, as you choose it on screen | **No** — the P&L step lists the same |
| `documents/01-accreditation-record.pdf` | Accreditation record and transfer condition | **Yes** — documents step |
| `documents/02-medicare-cost-report-summary.pdf` | Filed cost report summary: days, costs and committed regulatory capex | **Yes** — documents step |
| `documents/03-service-line-dependence.pdf` | Aggregate physician dependence by service line | **Yes** — documents step |
| `documents/04-management-presentation.pdf` | The seller's management presentation (the deck) | **Yes** — documents step |
| `documents/05-quality-reporting-summary.pdf` | Published quality-reporting summary | **Yes** — documents step |
| `documents/06-property-condition-assessment.pdf` | Property condition assessment of the hospital plant | **Yes** — documents step |
| `documents/07-payer-agreement-keystone.pdf` | Payer agreement: Commercial plan Keystone | **Yes** — documents step |
| `documents/08-payer-agreement-riverbend.pdf` | Payer agreement: Commercial plan Riverbend | **Yes** — documents step |
| `documents/09-transaction-timetable.pdf` | Transaction timetable | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `bidders.csv` | The three bidding firms for Part B: who to invite, what each asks and offers | **No** — read it while you follow Part B |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Notes

- Physician data is aggregate or pseudonymous (MS-001, MS-002, …); Pactlab never sends people data to a model.
- The checks reconcile documents, figures and dates; they make no clinical, survey or legal judgment.

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
| `02 Finance/Exports/St. capital spend history export Sep26.csv` | Capital spend history |  |
| `02 Finance/Exports/St. census export Sep26.csv` | Census |  |
| `02 Finance/Exports/St. invoice lines export Sep26.csv` | Invoice lines |  |
| `02 Finance/Exports/St. medical-staff roster export Sep26.csv` | Medical-staff roster |  |
| `02 Finance/Management presentation.pdf` | Other |  |
| `02 Finance/Medicare cost report summary.pdf` | Other |  |
| `02 Finance/Mgmt accounts FY26 - St..md` | Income statement (P&L) | Revenue matches the invoice lines for Oct 2025 – Sep 2026. |
| `02 Finance/Property condition assessment.pdf` | Other |  |
| `02 Finance/Quality reporting summary.pdf` | Other |  |
| `02 Finance/Service line dependence.pdf` | Other |  |
| `02 Finance/St. FY26 summary.md` | Pactlab asks: income statement or cash flow statement? | Mixes profit and cash flow lines. |
| `02 Finance/Transaction timetable.pdf` | Other |  |
| `03 Commercial/Customers/Payer agreement keystone (signed copy).pdf` | Duplicate — shown once | Same bytes as the agreement above. |
| `03 Commercial/Customers/Payer agreement keystone.pdf` | Customer contract |  |
| `03 Commercial/Customers/Payer agreement riverbend.pdf` | Customer contract |  |
| `04 Legal/Accreditation record.pdf` | Loan agreement |  |

**And on the Intake checklist**, these should show as missing: **Cash flow statement**, **Payer mix**.
Once billing is imported, **Customer contract** shows **Some missing** and names the largest billed customers with no contract in the room.
Click **Ask the seller** (or **Copy request for missing items**) to send the list.
