# Ashgrove Residential B.V. — Multifamily syndication (EUR)

**Fictional target.** Ashgrove Residential B.V. is a multifamily sponsor buying Briarwood Commons, a 204-unit garden-style community in six buildings (A–F), and raising the equity from accredited investors under Rule 506(c). The seller is Briarwood Commons Owner B.V..
Based in Utrecht, the Netherlands; reports in EUR. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Before you start

- Download this whole folder (on GitHub: **Code → Download ZIP** at the top of the repository, then unzip).
- Sign in to Pactlab. The steps take about 15 minutes.
- You upload **8 CSV files** and **5 PDFs**. Nothing else.
- **Never upload the `.md` files** in `documents/`. They are the text each PDF is built from; Pactlab reads the PDFs.
- `vdr-index.csv` is for reference only (how a data room would list these files). Do not upload it.
- Text in **bold** below is a button, tab or option exactly as Pactlab shows it.

## Two ways to test this company

- **Part A — Buyer side** (Steps 1 onwards): you are Ashgrove Residential B.V., the sponsor, diligencing the property you are buying and the offering you raise its equity on.
- **Part B — Seller side** ([below](#part-b--seller-side-run-a-bid-process)): you are Briarwood Commons Owner B.V., inviting several buyers — they ask questions, then offer or pass, and you choose one. Uses `bidders.csv`.
- Each part starts its own Pact, so you can do either one, or both.

# Part A — Buyer side

## Step 1 — Start the Pact

1. Click **Start a Pact** (top right).
2. **Name the Pact** — Pact name: `Project Ashgrove` · Base currency: **EUR** → **Next**.
3. **Buying entity** — Legal or trading name: `Ashgrove Residential B.V.` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `Briarwood Commons Owner B.V.` · **Private** · What kind of company is it?: **Multifamily syndication** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `40000000` (EUR 40,000,000) |
   | Currency | **EUR** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the seller's ask: 12× the September 2026 billed revenue run-rate. The demo shows how far the evidence supports it.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `Briarwood Commons Owner B.V.`, with the asking price EUR 40,000,000.

## Step 2 — Upload the billing export

1. Open the **Sources** tab → **Upload billing export**.
2. *1. Where is the export from?* → **Pactlab standard template**.
3. *2. Choose the file* → `invoice-lines.csv` → **Upload and map columns**.
4. The columns are matched for you. Click **Check every row**, then **Import 4344 lines**.

**You should see:** a green message ending "Finances now include them." The **Finances** tab now shows the revenue ledger.

## Step 3 — Upload the industry data

Open the **Sources** tab and scroll to **Industry data**. Upload these files one at a time:

| # | Click | Choose the file | Then | Button should read |
|---|---|---|---|---|
| 1 | **Upload rent roll** | `rent-roll.csv` | **Upload and map columns** → **Check every row** | **Import 204 rows** |
| 2 | **Upload t-12 operating statement** | `t12.csv` | **Upload and map columns** → **Check every row** | **Import 12 rows** |
| 3 | **Upload delinquency report** | `delinquency.csv` | **Upload and map columns** → **Check every row** | **Import 11 rows** |
| 4 | **Upload unit inspections** | `unit-inspections.csv` | **Upload and map columns** → **Check every row** | **Import 204 rows** |
| 5 | **Upload occupancy and rent history** | `occupancy-history.csv` | **Upload and map columns** → **Check every row** | **Import 60 rows** |
| 6 | **Upload rent roll snapshots** | `rent-roll-history.csv` | **Upload and map columns** → **Check every row** | **Import 1632 rows** |
| 7 | **Upload sponsor track record** | `track-record.csv` | **Upload and map columns** → **Check every row** | **Import 5 rows** |

**You should see** after each import: "… imported … Industry checks ran on them". Some findings may already appear as drafts; that is expected.

## Step 4 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/01-offering-memorandum.pdf` | **business information** | Seller's offering memorandum with stated NOI and capital plan |
| 2 | `documents/02-private-placement-memorandum.pdf` | **business information** | Private placement memorandum: the offering, fee summary, distributions and projected returns |
| 3 | `documents/03-operating-agreement.pdf` | **business information** | Operating agreement: fees, preferred return and promote |
| 4 | `documents/04-investor-deck.pdf` | **business information** | Sponsor's investor deck with its track record |
| 5 | `documents/99-data-room-extracts.pdf` | **financial information** | Every CSV extract in this folder as one paged PDF, so findings can cite a page |

**You should see:** all 5 documents listed on the **Documents** tab.

## Step 5 — Read the offering (Syndication tab)

Open the **Syndication** tab (it appears only on a multifamily syndication pact).

1. Under **The offering**, enter:

   | Field | Enter |
   |---|---|
   | Purchase price | `30600000` |
   | Loan | `19900000` |
   | Interest rate (%) | `5` |
   | Equity raised | `11800000` |
   | Hold (years) | `5` |
   | Selling costs (%) | `2` |
   | Year-1 NOI | leave empty (the T-12 is used) |
   | Exemption | **Rule 506(c)** |
   | NOI growth (%), downside / base / upside | `1` / `3` / `4.5` |
   | Exit cap rate (%), downside / base / upside | `6.5` / `6` / `5.5` |

   → **Save the offering**.
2. Under **Read the offering documents**, click **Read with AI** for `02-private-placement-memorandum.pdf` (PPM), `03-operating-agreement.pdf` (Operating agreement) and `04-investor-deck.pdf` (Investor deck).
3. Under **To confirm**, check each proposed term or claim against its quote, then **Confirm** it (or correct the figure first, or **Reject** it). Only confirmed items feed the waterfall.
4. Click **Run offering checks**.

**You should see:** **Waterfall check** with the base case recomputed from the operating agreement (investor IRR 9.67%, against the PPM's 14.3%), downside and upside alongside, each labelled as a scenario computed from stated assumptions; the **Track record** table with Stonebridge Flats' actual IRR shown as not documented; and three offering drafts on **Findings**.

## Step 6 — Upload the P&L by year

Open the **Sources** tab, scroll to **Industry data** and click **Upload profit and loss (p&l)**.

1. Choose `pnl.csv` → **Upload and map columns**. Pactlab reads the five years across the columns (FY2022 to FY2026).
2. Under **What each line is**, keep the two revenue lines as **Revenue** and every other line as **Operating expense** (the insurance refund is a credit, entered negative).
3. **Check every row**, then **Import 50 rows**.

**You should see:** on **Home → Property metrics**, a **History** strip under net operating income, occupancy and average rent, each with five points and "FY2022–FY2026 (5 years; earlier years not provided)"; on **Finances**, the five years side by side.

## Step 7 — Run the checks and review the findings

1. Open the **Findings** tab → **Run multifamily syndication checks**.
2. **You should see exactly these 12 findings** (running the checks again adds nothing):

   1. **Offering memorandum NOI above the T-12** — the seller's memorandum states EUR 2,036,471; `t12.csv` sums to EUR 1,834,659.
   2. **Deferred maintenance above the capital plan** — `unit-inspections.csv` estimates EUR 432,676 of repairs against a EUR 281,520 capital plan.
   3. **Delinquency concentrated in Building C** — 63.6% of delinquent units in `delinquency.csv` are in Building C.
   4. **Loss-to-lease (upside, not price)** — occupied units are 7.0% below market rent in `rent-roll.csv`.
   5. **Stated investor IRR inconsistent with the recomputed waterfall** — planted defect (a), on the **Syndication** tab: the PPM states 14.3%; the waterfall recomputed from the operating agreement on the base case gives 9.67% (`documents/02-private-placement-memorandum.pdf` page 5).
   6. **Track-record claim with no actuals behind it: Stonebridge Flats** — planted defect (b), on the **Syndication** tab: the deck claims 19.2%; `track-record.csv` has no actual return for it (`documents/04-investor-deck.pdf` page 2).
   7. **Fee in the operating agreement missing from the PPM: loan guarantee fee** — planted defect (c), on the **Syndication** tab: 1% of the loan in `documents/03-operating-agreement.pdf` page 2; the PPM fee summary (page 3) omits it.
   8. **Occupancy eroding, FY2022–FY2026** — planted: `occupancy-history.csv` — average occupancy FY2022 95.5%, FY2023 95.0%, FY2024 92.9%, FY2025 90.9%, FY2026 88.7%; below 90% in FY2026. The rent roll alone shows only today.
   9. **Repairs and maintenance growing faster than rent, FY2022–FY2026** — planted: `pnl.csv` and `occupancy-history.csv` — repairs and maintenance 8.4% a year (EUR 207,914 to EUR 287,421) against average rent 3.2% a year.
   10. **NOI jump in FY2026 above the history's trend** — planted: `pnl.csv` — NOI up 5.7% in FY2026 against an average of -2.0% a year before it, from deferred repairs and a one-off insurance refund of EUR 40,293; concessions rose too. The "dressed for sale" pattern.
   11. **P&L trend, 2022–2026** — `pnl.csv` — the five years side by side, a record for review.
   12. **Operating margin down across 2022–2026** — `pnl.csv` — NOI margin 58.0% in FY2022 to 54.6% in FY2026.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 8 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

# Part B — Seller side: run a bid process

Here you are Briarwood Commons Owner B.V. You invite three bidders from `bidders.csv`, share a little, answer their questions and choose one.
Each bidder sees only their own bid — never another bidder's questions, offers or whether they passed. Part B checks that too.

**Addresses.** This folder holds no email addresses. Invite **an address you can read for each firm**: your own address with `+` and the firm's tag from `bidders.csv` added before the @ (for tag `harbor`: *yourname+harbor* at your email domain — Gmail, Outlook and most providers deliver it to you). On your own computer (`pnpm dev`) any made-up address works: every email Pactlab sends, invitations and sign-in codes, is written to `apps/api/.data/mail/`.

## Step B1 — Start the Pact as the seller

1. Click **Start a Pact** (top right).
2. Under *Who are you in this deal?* choose **We are selling (or raising)**. Pact name: `Project Ashgrove Sale` · Base currency: **EUR** → **Next**. (There is no buying-entity step.)
3. **Selling entity** — Legal or trading name: `Briarwood Commons Owner B.V.` · **Private** · What kind of company is it?: **Multifamily syndication** → **Next**.
4. **Asking price** — enter the same asking price as Part A, Step 1 (`40000000`) → **Next**.
5. **Review and start** — the Buyer box says *Bid process — you invite buyers once the pact starts* → **Start Pact**.

**You should see:** the **Bidders** page, with no bidders yet.

## Step B2 — Decide what bidders see

On **Bidders**, under **What bidders see**:

| Field | Enter |
|---|---|
| Shared summary | `Briarwood Commons Owner B.V. is selling Briarwood Commons, a 204-unit garden-style apartment community in six buildings (A–F).` |
| Your data room (link) | `https://dataroom.example/multifamily-syndication` (Pactlab is not the data room; this is where you would grant access) |
| NDA | `Mutual NDA (synthetic): everything shared about Briarwood Commons Owner B.V. stays confidential.` |
| Offer deadline (UTC) | a date a week from today |

→ **Save**.

Then open the **Documents** tab and upload `documents/01-offering-memorandum.pdf` with **Share with bidders** ticked (it is chosen at upload and cannot be changed later). Upload nothing else as shared — the rest stays with you.

**You should see:** "Saved. Bidders see the shared view once they accept the NDA." On Documents, `01-offering-memorandum.pdf` is listed.

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
   | Price | `37000000` (EUR 37,000,000) |
   | Currency | `EUR` |
   | Structure (cash, shares, earn-out…) | `Cash at close for 100% of the shares` |
   | Conditions | `Subject to confirmatory diligence and committed financing` |

   → **Submit offer**.
3. **Northline Strategic (synthetic)**: ask `Can you share the last three years of audited accounts?` → **Ask**. Then offer **Price** `34000000` (EUR 34,000,000), **Structure** `80% cash at close, 20% earn-out over 24 months`, **Conditions** `Key-person retention for the founders` → **Submit offer**.
4. **Atlas Growth Equity (synthetic)**: accept the NDA, then type `Outside our sector focus this year.` as the reason → **Pass on this pact**.

**You should see**, as Northline Strategic (synthetic): your own question and offer only — nothing of Harbor Capital Partners (synthetic)'s question or offer, and no sign that Atlas Growth Equity (synthetic) passed. There are no deal tabs; trying `/deals/<id>/bidders` shows nothing of the seller's side.

## Step B5 — Answer the questions

Back as the seller (your normal window), on **Bidders** under **Questions from bidders**:

- Harbor Capital Partners (synthetic)'s question → answer `One customer contract has a change-of-control clause; it is in the shared documents.` → choose **All bidders (without naming who asked)** → **Answer**.
- Northline Strategic (synthetic)'s question → answer `FY2024 and FY2025 are audited; FY2026 closes in December. We will add them to the data room.` → keep **Only Northline Strategic (synthetic)** → **Answer**.

**You should see**, as Northline Strategic (synthetic) (refresh **Your bid**): your private answer, and under *Answered to all bidders* the change-of-control question — without the name of who asked it. Harbor Capital Partners (synthetic) sees the answer to all, but not Northline Strategic (synthetic)'s private one.

## Step B6 — Compare the offers

On **Bidders**, **Offers side by side** sets the two offers next to each other — price, structure, conditions, version. Pactlab does not rank them or recommend one.

**You should see:** Harbor Capital Partners (synthetic) at EUR 37,000,000 and Northline Strategic (synthetic) at EUR 34,000,000; Atlas Growth Equity (synthetic) marked **Passed** with its reason.

## Step B7 — Shortlist, run round 2 and choose

1. Click **Shortlist** on Harbor Capital Partners (synthetic) and on Northline Strategic (synthetic), then **Start round 2 with 2 shortlisted**.
2. As each bidder, submit a revised offer on **Your bid**: Harbor Capital Partners (synthetic) `39000000`, Northline Strategic (synthetic) `35000000` → **Submit revised offer**. Every version stays listed.
3. As the seller, click **Award to Harbor Capital Partners (synthetic)**.

**You should see:** "Awarded. Every other bidder has been declined and their access ended." Harbor Capital Partners (synthetic)'s **Your bid** says **Selected by the seller**; Northline Strategic (synthetic) can no longer open the pact. The **Team** tab and the audit log record every step.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 4344 revenue lines, one per unit rent charge per month | **Yes** — billing export step |
| `rent-roll.csv` | Rent roll at 30 September 2026 (204 rows) | **Yes** — industry data step |
| `delinquency.csv` | Delinquent balances at 30 September 2026 (11 rows) | **Yes** — industry data step |
| `unit-inspections.csv` | Unit-condition inspections with repair estimates (204 rows) | **Yes** — industry data step |
| `operating-statements-monthly.csv` | Operating statements by month, October 2021 to September 2026 (one row per line per month) (600 rows) | **No** — it is already inside `documents/99-data-room-extracts.pdf`, which you upload |
| `pnl.csv` | Operating statement by fiscal year (October to September), FY2022 to FY2026 (10 lines) | **Yes** — P&L step |
| `occupancy-history.csv` | Occupancy and average in-place rent by month, October 2021 to September 2026 (60 rows) | **Yes** — industry data step |
| `rent-roll-history.csv` | Rent-roll snapshots at each quarter end, December 2024 to September 2026 (1632 rows) | **Yes** — industry data step |
| `t12.csv` | Trailing-twelve-month operating statement (T-12) (12 rows) | **Yes** — industry data step |
| `track-record.csv` | Sponsor's track record: prior deals, projected and actual (5 rows) | **Yes** — industry data step |
| `documents/01-offering-memorandum.pdf` | Seller's offering memorandum with stated NOI and capital plan | **Yes** — documents step |
| `documents/02-private-placement-memorandum.pdf` | Private placement memorandum: the offering, fee summary, distributions and projected returns | **Yes** — documents step |
| `documents/03-operating-agreement.pdf` | Operating agreement: fees, preferred return and promote | **Yes** — documents step |
| `documents/04-investor-deck.pdf` | Sponsor's investor deck with its track record | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `bidders.csv` | The three bidding firms for Part B: who to invite, what each asks and offers | **No** — read it while you follow Part B |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Notes

- Sponsor-side pack: you are the sponsor. The property side is the Multifamily pack, unchanged; the offering side reads the PPM, operating agreement and deck on the **Syndication** tab: **Read with AI** on each, confirm what it proposes, then **Run offering checks**.
- Offering terms for the **Syndication** tab: purchase price `30600000`, loan `19900000` at `5`%, equity raised `11800000`, hold `5` years, selling costs `2`%, Rule 506(c); paths (NOI growth / exit cap %): downside `1` / `6.5`, base `3` / `6`, upside `4.5` / `5.5`. Leave year-1 NOI empty to use the T-12.
- The waterfall recomputed on the base case: investor IRR 9.67%, equity multiple 1.53x, average cash-on-cash 6.08%. The multiple and cash-on-cash the PPM states agree; the IRR does not.
- Planted defect (d), a property finding the sponsor does not publish to investors, arrives with the investor view (T-106 PR 2).
- Diligence support only: not legal advice, no accreditation determination, no securities-offering or broker-dealer function.
- History (T-183): five fiscal years, October to September, FY2022 to FY2026; FY2026 is the T-12, so `t12.csv` equals the last twelve months of `operating-statements-monthly.csv` and of `pnl.csv`'s FY2026 column, and the September 2026 month of `occupancy-history.csv` matches `rent-roll.csv`.
- Figures the history checks reproduce: NOI growth -0.2% a year and revenue growth 1.4% a year (FY2022–FY2026); average in-place rent FY2022 EUR 1,344.09, FY2023 EUR 1,387.10, FY2024 EUR 1,431.48, FY2025 EUR 1,477.29, FY2026 EUR 1,524.56 (3.2% a year); occupancy FY2022 95.5%, FY2023 95.0%, FY2024 92.9%, FY2025 90.9%, FY2026 88.7%; expense ratio 45.4% in FY2026; trailing three-year vacancy 9.1%.
- `operating-statements-monthly.csv` is the same statement as a long file (one row per line per month); it imports through the same P&L import. `rent-roll-history.csv` holds quarterly rent-roll snapshots for the last two years.

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
| `02 Finance/Ashgrove FY26 summary.md` | Pactlab asks: income statement or cash flow statement? | Mixes profit and cash flow lines. |
| `02 Finance/Exports/Ashgrove delinquency report export Sep26.csv` | Delinquency report |  |
| `02 Finance/Exports/Ashgrove invoice lines export Sep26.csv` | Invoice lines |  |
| `02 Finance/Exports/Ashgrove occupancy and rent history export Sep26.csv` | Occupancy and rent history |  |
| `02 Finance/Exports/Ashgrove profit and loss (p&l) export Sep26.csv` | Profit and loss (P&L) |  |
| `02 Finance/Exports/Ashgrove rent roll export Sep26.csv` | Rent roll |  |
| `02 Finance/Exports/Ashgrove rent roll snapshots export Sep26.csv` | Rent roll snapshots |  |
| `02 Finance/Exports/Ashgrove t-12 operating statement export Sep26.csv` | T-12 operating statement |  |
| `02 Finance/Investor deck.pdf` | Other |  |
| `02 Finance/Mgmt accounts FY26 - Ashgrove.md` | Income statement (P&L) | Revenue matches the invoice lines for Oct 2025 – Sep 2026. |
| `02 Finance/Offering memorandum.pdf` | Other |  |
| `02 Finance/Private placement memorandum.pdf` | Other |  |
| `03 Commercial/Customers/Operating agreement (signed copy).pdf` | Duplicate — shown once | Same bytes as the agreement above. |
| `03 Commercial/Customers/Operating agreement.pdf` | Customer contract |  |

**And on the Intake checklist**, these should show as missing: **Cash flow statement**, **Unit inspections**.
Once billing is imported, **Customer contract** shows **Some missing** and names the largest billed customers with no contract in the room.
Click **Ask the seller** (or **Copy request for missing items**) to send the list.
