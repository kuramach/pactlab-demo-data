# Quayside Estates Inc. — Commercial property (USD)

**Fictional target.** Quayside Estates Inc. owns Quayside Business Park, a 361,000 sq ft mixed office and light-industrial park, fully let to eleven tenants on triple-net leases.
Based in Columbus, Ohio, United States; reports in USD. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Before you start

- Download this whole folder (on GitHub: **Code → Download ZIP** at the top of the repository, then unzip).
- Sign in to Pactlab. The steps take about 15 minutes.
- You upload **4 CSV files** and **16 PDFs**. Nothing else.
- **Never upload the `.md` files** in `documents/`. They are the text each PDF is built from; Pactlab reads the PDFs.
- `vdr-index.csv` is for reference only (how a data room would list these files). Do not upload it.
- Text in **bold** below is a button, tab or option exactly as Pactlab shows it.

## Two ways to test this company

- **Part A — Buyer side** (Steps 1 onwards): you are a buyer doing diligence on Quayside Estates Inc..
- **Part B — Seller side** ([below](#part-b--seller-side-run-a-bid-process)): you are Quayside Estates Inc., inviting several buyers — they ask questions, then offer or pass, and you choose one. Uses `bidders.csv`.
- Each part starts its own Pact, so you can do either one, or both.

# Part A — Buyer side

## Step 1 — Start the Pact

1. Click **Start a Pact** (top right).
2. **Name the Pact** — Pact name: `Project Quayside` · Base currency: **USD** → **Next**.
3. **Buying entity** — Legal or trading name: `Demo Buyer` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `Quayside Estates Inc.` · **Private** · What kind of company is it?: **Commercial property** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `26000000` (USD 26,000,000) |
   | Currency | **USD** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the seller's ask: 11× the September 2026 billed revenue run-rate. The demo shows how far the evidence supports it.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `Quayside Estates Inc.`, with the asking price USD 26,000,000.

## Step 2 — Upload the billing export

1. Open the **Sources** tab → **Upload billing export**.
2. *1. Where is the export from?* → **Pactlab standard template**.
3. *2. Choose the file* → `invoice-lines.csv` → **Upload and map columns**.
4. The columns are matched for you. Click **Check every row**, then **Import 264 lines**.

**You should see:** a green message ending "Finances now include them." The **Finances** tab now shows the revenue ledger.

## Step 3 — Upload the industry data

Open the **Sources** tab and scroll to **Industry data**. Upload these files one at a time:

| # | Click | Choose the file | Then | Button should read |
|---|---|---|---|---|
| 1 | **Upload commercial rent roll** | `rent-roll.csv` | **Upload and map columns** → **Check every row** | **Import 11 rows** |
| 2 | **Upload cam reconciliation** | `cam-reconciliation.csv` | **Upload and map columns** → **Check every row** | **Import 12 rows** |
| 3 | **Upload capex schedule** | `capex-schedule.csv` | **Upload and map columns** → **Check every row** | **Import 3 rows** |

**You should see** after each import: "… imported … Industry checks ran on them". Some findings may already appear as drafts; that is expected.

## Step 4 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/03-lease-unit-01.pdf` | **business information** | Lease for Unit 1: term, rent, escalation and recoveries |
| 2 | `documents/03-lease-unit-02.pdf` | **business information** | Lease for Unit 2: term, rent, escalation and recoveries |
| 3 | `documents/03-lease-unit-03.pdf` | **business information** | Lease for Unit 3: term, rent, escalation and recoveries |
| 4 | `documents/03-lease-unit-04.pdf` | **business information** | Lease for Unit 4: term, rent, escalation and recoveries |
| 5 | `documents/03-lease-unit-05.pdf` | **business information** | Lease for Unit 5: term, rent, escalation and recoveries |
| 6 | `documents/03-lease-unit-06.pdf` | **business information** | Lease for Unit 6: term, rent, escalation and recoveries |
| 7 | `documents/03-lease-unit-07.pdf` | **business information** | Lease for Unit 7: term, rent, escalation and recoveries |
| 8 | `documents/03-lease-unit-08.pdf` | **business information** | Lease for Unit 8: term, rent, escalation and recoveries |
| 9 | `documents/03-lease-unit-09.pdf` | **business information** | Lease for Unit 9: term, rent, escalation and recoveries |
| 10 | `documents/03-lease-unit-10.pdf` | **business information** | Lease for Unit 10: term, rent, escalation and recoveries |
| 11 | `documents/03-lease-unit-11.pdf` | **business information** | Lease for Unit 11: term, rent, escalation and recoveries |
| 12 | `documents/01-phase-i-environmental-site-assessment.pdf` | **business information** | Phase I environmental site assessment |
| 13 | `documents/02-lease-abstract-corvane.pdf` | **business information** | Lease abstract for the anchor tenant |
| 14 | `documents/04-property-condition-assessment.pdf` | **business information** | Engineer’s property condition assessment: flagged items and estimated costs |
| 15 | `documents/05-offering-memorandum.pdf` | **business information** | Offering memorandum: occupancy, the closing date and the hold |
| 16 | `documents/99-data-room-extracts.pdf` | **financial information** | Every CSV extract in this folder as one paged PDF, so findings can cite a page |

**You should see:** all 16 documents listed on the **Documents** tab.

## Step 5 — Upload the P&L by year

Open the **Sources** tab, scroll to **Industry data** and click **Upload profit and loss (p&l)**.

1. Choose `pnl.csv` → **Upload and map columns**. Pactlab reads the three years across the columns (FY2023 to FY2025).
2. Say what each line is: the two lines ending in *revenue* are **Revenue**, and the rest are **Operating expenses**.
3. **Check every row**, then **Import 24 rows**.

**You should see:** the import succeed. **Finances** shows the three years side by side with the recovery ratio, and asks the seller for FY2021 and FY2022.

## Step 6 — Run the checks and review the findings

1. Open the **Findings** tab → **Run commercial property checks**.
2. **You should see exactly these 11 findings** (running the checks again adds nothing):

   1. **Anchor tenant concentration and near-term expiry** — Corvane Logistics (synthetic) is 41.0% of base rent and its lease ends 30 June 2027 (`rent-roll.csv`, `documents/02-lease-abstract-corvane.pdf`). Weighted average lease term is 2.3 years.
   2. **Recognized environmental condition** — `documents/01-phase-i-environmental-site-assessment.pdf` page 2 — former dry cleaner at Unit 9; Phase II recommended.
   3. **CAM recoveries below expenses** — `cam-reconciliation.csv` — repairs and security recover less than they cost in 2025.
   4. **Below-market anchor rent** — Corvane pays about 6% below market rent in `rent-roll.csv` — the deepest discount on the rent roll, on the largest lease.
   5. **Rent roll overstates rent against the leases: 2 tenants** — `rent-roll.csv` against `documents/03-lease-unit-02.pdf` and `documents/03-lease-unit-03.pdf` — Pellham Engineering (synthetic) by USD 1,103.88 a month and Brightwater Analytics (synthetic) by USD 1,500.00 a month; the FY2025 statements in `pnl.csv` carry the leases’ rent, USD 2,238,042.
   6. **NNN recoveries short of the leases in every year, 2023–2025** — `cam-reconciliation.csv` against the leases’ proportionate shares (100% triple net) — 2023: USD 36,000 short, 2024: USD 50,000 short, 2025: USD 64,000 short. A single year looks like timing; three in a row is a leak.
   7. **Landlord obligations the buyer inherits: tenant improvements, leasing commissions and committed capex** — the unpaid tenant improvements on Unit 2, the Gullwing leasing commission and the committed lines of `capex-schedule.csv`: USD 754,000 in all, priced as a credit at closing.
   8. **Rent cliff: Corvane Logistics (synthetic) (41.0% of rent) expires in year 1 of the hold** — `rent-roll.csv` and `documents/03-lease-unit-01.pdf` — the largest tenant ends on 30 June 2027, six months after the 31 December 2026 closing in `documents/05-offering-memorandum.pdf`.
   9. **Roof work flagged by the condition report is not in the seller’s capex schedule** — `documents/04-property-condition-assessment.pdf` — roof replacement within two years at USD 1,850,000; `capex-schedule.csv` has no roof line. Priced as remediation.
   10. **P&L trend, 2023–2025** — every imported year side by side: revenue, growth, margins and the repairs, taxes and insurance ratios.
   11. **Repairs and maintenance growing faster than revenue, 2023–2025** — repairs and maintenance rise from 5.9% to 7.6% of revenue — FY2025 alone looks ordinary.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 7 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

# Part B — Seller side: run a bid process

Here you are Quayside Estates Inc. You invite three bidders from `bidders.csv`, share a little, answer their questions and choose one.
Each bidder sees only their own bid — never another bidder's questions, offers or whether they passed. Part B checks that too.

**Addresses.** This folder holds no email addresses. Invite **an address you can read for each firm**: your own address with `+` and the firm's tag from `bidders.csv` added before the @ (for tag `harbor`: *yourname+harbor* at your email domain — Gmail, Outlook and most providers deliver it to you). On your own computer (`pnpm dev`) any made-up address works: every email Pactlab sends, invitations and sign-in codes, is written to `apps/api/.data/mail/`.

## Step B1 — Start the Pact as the seller

1. Click **Start a Pact** (top right).
2. Under *Who are you in this deal?* choose **We are selling (or raising)**. Pact name: `Project Quayside Sale` · Base currency: **USD** → **Next**. (There is no buying-entity step.)
3. **Selling entity** — Legal or trading name: `Quayside Estates Inc.` · **Private** · What kind of company is it?: **Commercial property** → **Next**.
4. **Asking price** — enter the same asking price as Part A, Step 1 (`26000000`) → **Next**.
5. **Review and start** — the Buyer box says *Bid process — you invite buyers once the pact starts* → **Start Pact**.

**You should see:** the **Bidders** page, with no bidders yet.

## Step B2 — Decide what bidders see

On **Bidders**, under **What bidders see**:

| Field | Enter |
|---|---|
| Shared summary | `Quayside Estates Inc. owns Quayside Business Park, a 361,000 sq ft mixed office and light-industrial park, fully let to eleven tenants on triple-net leases.` |
| Your data room (link) | `https://dataroom.example/commercial-property` (Pactlab is not the data room; this is where you would grant access) |
| NDA | `Mutual NDA (synthetic): everything shared about Quayside Estates Inc. stays confidential.` |
| Offer deadline (UTC) | a date a week from today |

→ **Save**.

Then open the **Documents** tab and upload `documents/03-lease-unit-01.pdf` with **Share with bidders** ticked (it is chosen at upload and cannot be changed later). Upload nothing else as shared — the rest stays with you.

**You should see:** "Saved. Bidders see the shared view once they accept the NDA." On Documents, `03-lease-unit-01.pdf` is listed.

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
   | Price | `24000000` (USD 24,000,000) |
   | Currency | `USD` |
   | Structure (cash, shares, earn-out…) | `Cash at close for 100% of the shares` |
   | Conditions | `Subject to confirmatory diligence and committed financing` |

   → **Submit offer**.
3. **Northline Strategic (synthetic)**: ask `Can you share the last three years of audited accounts?` → **Ask**. Then offer **Price** `22000000` (USD 22,000,000), **Structure** `80% cash at close, 20% earn-out over 24 months`, **Conditions** `Key-person retention for the founders` → **Submit offer**.
4. **Atlas Growth Equity (synthetic)**: accept the NDA, then type `Outside our sector focus this year.` as the reason → **Pass on this pact**.

**You should see**, as Northline Strategic (synthetic): your own question and offer only — nothing of Harbor Capital Partners (synthetic)'s question or offer, and no sign that Atlas Growth Equity (synthetic) passed. There are no deal tabs; trying `/deals/<id>/bidders` shows nothing of the seller's side.

## Step B5 — Answer the questions

Back as the seller (your normal window), on **Bidders** under **Questions from bidders**:

- Harbor Capital Partners (synthetic)'s question → answer `One customer contract has a change-of-control clause; it is in the shared documents.` → choose **All bidders (without naming who asked)** → **Answer**.
- Northline Strategic (synthetic)'s question → answer `FY2024 and FY2025 are audited; FY2026 closes in December. We will add them to the data room.` → keep **Only Northline Strategic (synthetic)** → **Answer**.

**You should see**, as Northline Strategic (synthetic) (refresh **Your bid**): your private answer, and under *Answered to all bidders* the change-of-control question — without the name of who asked it. Harbor Capital Partners (synthetic) sees the answer to all, but not Northline Strategic (synthetic)'s private one.

## Step B6 — Compare the offers

On **Bidders**, **Offers side by side** sets the two offers next to each other — price, structure, conditions, version. Pactlab does not rank them or recommend one.

**You should see:** Harbor Capital Partners (synthetic) at USD 24,000,000 and Northline Strategic (synthetic) at USD 22,000,000; Atlas Growth Equity (synthetic) marked **Passed** with its reason.

## Step B7 — Shortlist, run round 2 and choose

1. Click **Shortlist** on Harbor Capital Partners (synthetic) and on Northline Strategic (synthetic), then **Start round 2 with 2 shortlisted**.
2. As each bidder, submit a revised offer on **Your bid**: Harbor Capital Partners (synthetic) `25000000`, Northline Strategic (synthetic) `23000000` → **Submit revised offer**. Every version stays listed.
3. As the seller, click **Award to Harbor Capital Partners (synthetic)**.

**You should see:** "Awarded. Every other bidder has been declined and their access ended." Harbor Capital Partners (synthetic)'s **Your bid** says **Selected by the seller**; Northline Strategic (synthetic) can no longer open the pact. The **Team** tab and the audit log record every step.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 264 revenue lines, one per tenant base-rent charge per month | **Yes** — billing export step |
| `rent-roll.csv` | Commercial rent roll with expiries and market rents (11 rows) | **Yes** — industry data step |
| `cam-reconciliation.csv` | Recoverable expenses against tenant recoveries billed, by year and category (12 rows) | **Yes** — industry data step |
| `capex-schedule.csv` | The seller’s capital expenditure schedule: item, element, amount and status (3 rows) | **Yes** — industry data step |
| `pnl.csv` | Profit and loss by fiscal year, FY2023 to FY2025 (8 lines) | **Yes** — P&L step |
| `documents/03-lease-unit-01.pdf` | Lease for Unit 1: term, rent, escalation and recoveries | **Yes** — documents step |
| `documents/03-lease-unit-02.pdf` | Lease for Unit 2: term, rent, escalation and recoveries | **Yes** — documents step |
| `documents/03-lease-unit-03.pdf` | Lease for Unit 3: term, rent, escalation and recoveries | **Yes** — documents step |
| `documents/03-lease-unit-04.pdf` | Lease for Unit 4: term, rent, escalation and recoveries | **Yes** — documents step |
| `documents/03-lease-unit-05.pdf` | Lease for Unit 5: term, rent, escalation and recoveries | **Yes** — documents step |
| `documents/03-lease-unit-06.pdf` | Lease for Unit 6: term, rent, escalation and recoveries | **Yes** — documents step |
| `documents/03-lease-unit-07.pdf` | Lease for Unit 7: term, rent, escalation and recoveries | **Yes** — documents step |
| `documents/03-lease-unit-08.pdf` | Lease for Unit 8: term, rent, escalation and recoveries | **Yes** — documents step |
| `documents/03-lease-unit-09.pdf` | Lease for Unit 9: term, rent, escalation and recoveries | **Yes** — documents step |
| `documents/03-lease-unit-10.pdf` | Lease for Unit 10: term, rent, escalation and recoveries | **Yes** — documents step |
| `documents/03-lease-unit-11.pdf` | Lease for Unit 11: term, rent, escalation and recoveries | **Yes** — documents step |
| `documents/01-phase-i-environmental-site-assessment.pdf` | Phase I environmental site assessment | **Yes** — documents step |
| `documents/02-lease-abstract-corvane.pdf` | Lease abstract for the anchor tenant | **Yes** — documents step |
| `documents/04-property-condition-assessment.pdf` | Engineer’s property condition assessment: flagged items and estimated costs | **Yes** — documents step |
| `documents/05-offering-memorandum.pdf` | Offering memorandum: occupancy, the closing date and the hold | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `bidders.csv` | The three bidding firms for Part B: who to invite, what each asks and offers | **No** — read it while you follow Part B |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Notes

- Tenants are businesses; the rent roll is lease data, never people data.
- The eleven leases in `documents/` are what the rent roll is checked against: initial rent, escalation, term and each tenant’s proportionate share of recoverable expenses.
- `pnl.csv` and `cam-reconciliation.csv` hold FY2023–FY2025, read side by side on **Finances**; Pactlab asks the seller for FY2021 and FY2022.
- Diligence support only: the pack reconciles documents and arithmetic. It never values the property.

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
| `02 Finance/Exports/Quayside cam reconciliation export Sep26.csv` | CAM reconciliation |  |
| `02 Finance/Exports/Quayside invoice lines export Sep26.csv` | Invoice lines |  |
| `02 Finance/Mgmt accounts FY26 - Quayside.md` | Income statement (P&L) | Revenue matches the invoice lines for Oct 2025 – Sep 2026. |
| `02 Finance/Offering memorandum.pdf` | Other |  |
| `02 Finance/Phase i environmental site assessment.pdf` | Other |  |
| `02 Finance/Property condition assessment.pdf` | Other |  |
| `02 Finance/Quayside FY26 summary.md` | Pactlab asks: income statement or cash flow statement? | Mixes profit and cash flow lines. |
| `03 Commercial/Leases/Lease abstract corvane.pdf` | Lease |  |
| `03 Commercial/Leases/Lease unit 01.pdf` | Lease |  |
| `03 Commercial/Leases/Lease unit 02.pdf` | Lease |  |
| `03 Commercial/Leases/Lease unit 03.pdf` | Lease |  |
| `03 Commercial/Leases/Lease unit 04.pdf` | Lease |  |
| `03 Commercial/Leases/Lease unit 05.pdf` | Lease |  |
| `03 Commercial/Leases/Lease unit 06.pdf` | Lease |  |
| `03 Commercial/Leases/Lease unit 07.pdf` | Lease |  |
| `03 Commercial/Leases/Lease unit 08.pdf` | Lease |  |
| `03 Commercial/Leases/Lease unit 09.pdf` | Lease |  |
| `03 Commercial/Leases/Lease unit 10.pdf` | Lease |  |
| `03 Commercial/Leases/Lease unit 11.pdf` | Lease |  |

**And on the Intake checklist**, these should show as missing: **Cash flow statement**, **Rent roll**.
Once billing is imported, **Customer contract** shows **Some missing** and names the largest billed customers with no contract in the room.
Click **Ask the seller** (or **Copy request for missing items**) to send the list.
