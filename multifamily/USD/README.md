# Larkfield Residential Inc. — Multifamily (USD)

**Fictional target.** Larkfield Residential Inc. owns Larkfield Commons, a 96-unit garden-style apartment community in three buildings (A, B, C).
Based in Columbus, Ohio, United States; reports in USD. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Before you start

- Download this whole folder (on GitHub: **Code → Download ZIP** at the top of the repository, then unzip).
- Sign in to Pactlab. The steps take about 15 minutes.
- You upload **7 CSV files** and **2 PDFs**. Nothing else.
- **Never upload the `.md` files** in `documents/`. They are the text each PDF is built from; Pactlab reads the PDFs.
- `vdr-index.csv` is for reference only (how a data room would list these files). Do not upload it.
- Text in **bold** below is a button, tab or option exactly as Pactlab shows it.

## Two ways to test this company

- **Part A — Buyer side** (Steps 1 onwards): you are a buyer doing diligence on Larkfield Residential Inc..
- **Part B — Seller side** ([below](#part-b--seller-side-run-a-bid-process)): you are Larkfield Residential Inc., inviting several buyers — they ask questions, then offer or pass, and you choose one. Uses `bidders.csv`.
- Each part starts its own Pact, so you can do either one, or both.

# Part A — Buyer side

## Step 1 — Start the Pact

1. Click **Start a Pact** (top right).
2. **Name the Pact** — Pact name: `Project Larkfield` · Base currency: **USD** → **Next**.
3. **Buying entity** — Legal or trading name: `Demo Buyer` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `Larkfield Residential Inc.` · **Private** · What kind of company is it?: **Multifamily** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `21000000` (USD 21,000,000) |
   | Currency | **USD** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the seller's ask: 12× the September 2026 billed revenue run-rate. The demo shows how far the evidence supports it.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `Larkfield Residential Inc.`, with the asking price USD 21,000,000.

## Step 2 — Upload the billing export

1. Open the **Sources** tab → **Upload billing export**.
2. *1. Where is the export from?* → **Pactlab standard template**.
3. *2. Choose the file* → `invoice-lines.csv` → **Upload and map columns**.
4. The columns are matched for you. Click **Check every row**, then **Import 2040 lines**.

**You should see:** a green message ending "Finances now include them." The **Finances** tab now shows the revenue ledger.

## Step 3 — Upload the industry data

Open the **Sources** tab and scroll to **Industry data**. Upload these files one at a time:

| # | Click | Choose the file | Then | Button should read |
|---|---|---|---|---|
| 1 | **Upload rent roll** | `rent-roll.csv` | **Upload and map columns** → **Check every row** | **Import 96 rows** |
| 2 | **Upload t-12 operating statement** | `t12.csv` | **Upload and map columns** → **Check every row** | **Import 12 rows** |
| 3 | **Upload delinquency report** | `delinquency.csv` | **Upload and map columns** → **Check every row** | **Import 5 rows** |
| 4 | **Upload unit inspections** | `unit-inspections.csv` | **Upload and map columns** → **Check every row** | **Import 96 rows** |
| 5 | **Upload occupancy and rent history** | `occupancy-history.csv` | **Upload and map columns** → **Check every row** | **Import 240 rows** |
| 6 | **Upload rent roll snapshots** | `rent-roll-history.csv` | **Upload and map columns** → **Check every row** | **Import 768 rows** |

**You should see** after each import: "… imported … Industry checks ran on them". Some findings may already appear as drafts; that is expected.

## Step 4 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/01-offering-memorandum.pdf` | **business information** | Offering memorandum with stated NOI and capital plan |
| 2 | `documents/99-data-room-extracts.pdf` | **financial information** | Every CSV extract in this folder as one paged PDF, so findings can cite a page |

**You should see:** all 2 documents listed on the **Documents** tab.

## Step 5 — Upload the P&L by year

Open the **Sources** tab, scroll to **Industry data** and click **Upload profit and loss (p&l)**.

1. Choose `pnl.csv` → **Upload and map columns**. Pactlab reads the twenty years across the columns (FY2007 to FY2026).
2. Under **What each line is**, keep the two revenue lines as **Revenue** and every other line as **Operating expense** (the insurance refund is a credit, entered negative).
3. **Check every row**, then **Import 200 rows**.

**You should see:** on **Home → Property metrics**, a **History** strip under net operating income, occupancy and average rent, each with the last ten years and "FY2007–FY2026 (20 years)"; on **Finances**, every year side by side (the table scrolls), with the long-run figures beside the five-year ones.

## Step 6 — Run the checks and review the findings

1. Open the **Findings** tab → **Run multifamily checks**.
2. **You should see exactly these 10 findings** (running the checks again adds nothing):

   1. **Offering memorandum NOI above the T-12** — the memorandum states USD 1,102,241; `t12.csv` sums to USD 993,010 — the memorandum uses pro-forma rents.
   2. **Deferred maintenance above the capital plan** — `unit-inspections.csv` estimates USD 232,100 of repairs against a USD 144,000 capital plan — USD 2,418 per door. Price as remediation.
   3. **Delinquency concentrated in Building C** — 100.0% of delinquent units in `delinquency.csv` are in Building C.
   4. **Loss-to-lease (upside, not price)** — occupied units are 6.8% below market rent in `rent-roll.csv`. Record it as confirmed value — never as a reason to pay more.
   5. **Occupancy eroding, FY2022–FY2026** — planted: `occupancy-history.csv` — average occupancy FY2022 95.3%, FY2023 95.1%, FY2024 93.1%, FY2025 91.2%, FY2026 88.5%; below 90% in FY2026. The rent roll alone shows only today.
   6. **Repairs and maintenance growing faster than rent, FY2022–FY2026** — planted: `pnl.csv` and `occupancy-history.csv` — repairs and maintenance 8.4% a year (USD 112,534 to USD 155,567) against average rent 3.2% a year.
   7. **NOI jump in FY2026 above the history's trend** — planted: `pnl.csv` — NOI up 4.9% in FY2026 against an average of -1.7% a year before it, from deferred repairs and a one-off insurance refund of USD 21,808; concessions rose too. The "dressed for sale" pattern.
   8. **P&L trend, 2022–2026** — `pnl.csv` — the five years side by side, a record for review.
   9. **Operating margin down across 2022–2026** — `pnl.csv` — NOI margin 58.0% in FY2022 to 54.6% in FY2026.
   10. **The recent run is better than the long run: NOI margin, FY2022–FY2026 against FY2007–FY2026** — planted (T-185): `pnl.csv` — the NOI margin averaged 55.3% across FY2022–FY2026, against 46.4% across the twenty years. Ask whether the price assumes the recent run will last.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 7 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

# Part B — Seller side: run a bid process

Here you are Larkfield Residential Inc. You invite three bidders from `bidders.csv`, share a little, answer their questions and choose one.
Each bidder sees only their own bid — never another bidder's questions, offers or whether they passed. Part B checks that too.

**Addresses.** This folder holds no email addresses. Invite **an address you can read for each firm**: your own address with `+` and the firm's tag from `bidders.csv` added before the @ (for tag `harbor`: *yourname+harbor* at your email domain — Gmail, Outlook and most providers deliver it to you). On your own computer (`pnpm dev`) any made-up address works: every email Pactlab sends, invitations and sign-in codes, is written to `apps/api/.data/mail/`.

## Step B1 — Start the Pact as the seller

1. Click **Start a Pact** (top right).
2. Under *Who are you in this deal?* choose **We are selling (or raising)**. Pact name: `Project Larkfield Sale` · Base currency: **USD** → **Next**. (There is no buying-entity step.)
3. **Selling entity** — Legal or trading name: `Larkfield Residential Inc.` · **Private** · What kind of company is it?: **Multifamily** → **Next**.
4. **Asking price** — enter the same asking price as Part A, Step 1 (`21000000`) → **Next**.
5. **Review and start** — the Buyer box says *Bid process — you invite buyers once the pact starts* → **Start Pact**.

**You should see:** the **Bidders** page, with no bidders yet.

## Step B2 — Decide what bidders see

On **Bidders**, under **What bidders see**:

| Field | Enter |
|---|---|
| Shared summary | `Larkfield Residential Inc. owns Larkfield Commons, a 96-unit garden-style apartment community in three buildings (A, B, C).` |
| Your data room (link) | `https://dataroom.example/multifamily` (Pactlab is not the data room; this is where you would grant access) |
| NDA | `Mutual NDA (synthetic): everything shared about Larkfield Residential Inc. stays confidential.` |
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
   | Price | `19000000` (USD 19,000,000) |
   | Currency | `USD` |
   | Structure (cash, shares, earn-out…) | `Cash at close for 100% of the shares` |
   | Conditions | `Subject to confirmatory diligence and committed financing` |

   → **Submit offer**.
3. **Northline Strategic (synthetic)**: ask `Can you share the last three years of audited accounts?` → **Ask**. Then offer **Price** `18000000` (USD 18,000,000), **Structure** `80% cash at close, 20% earn-out over 24 months`, **Conditions** `Key-person retention for the founders` → **Submit offer**.
4. **Atlas Growth Equity (synthetic)**: accept the NDA, then type `Outside our sector focus this year.` as the reason → **Pass on this pact**.

**You should see**, as Northline Strategic (synthetic): your own question and offer only — nothing of Harbor Capital Partners (synthetic)'s question or offer, and no sign that Atlas Growth Equity (synthetic) passed. There are no deal tabs; trying `/deals/<id>/bidders` shows nothing of the seller's side.

## Step B5 — Answer the questions

Back as the seller (your normal window), on **Bidders** under **Questions from bidders**:

- Harbor Capital Partners (synthetic)'s question → answer `One customer contract has a change-of-control clause; it is in the shared documents.` → choose **All bidders (without naming who asked)** → **Answer**.
- Northline Strategic (synthetic)'s question → answer `FY2024 and FY2025 are audited; FY2026 closes in December. We will add them to the data room.` → keep **Only Northline Strategic (synthetic)** → **Answer**.

**You should see**, as Northline Strategic (synthetic) (refresh **Your bid**): your private answer, and under *Answered to all bidders* the change-of-control question — without the name of who asked it. Harbor Capital Partners (synthetic) sees the answer to all, but not Northline Strategic (synthetic)'s private one.

## Step B6 — Compare the offers

On **Bidders**, **Offers side by side** sets the two offers next to each other — price, structure, conditions, version. Pactlab does not rank them or recommend one.

**You should see:** Harbor Capital Partners (synthetic) at USD 19,000,000 and Northline Strategic (synthetic) at USD 18,000,000; Atlas Growth Equity (synthetic) marked **Passed** with its reason.

## Step B7 — Shortlist, run round 2 and choose

1. Click **Shortlist** on Harbor Capital Partners (synthetic) and on Northline Strategic (synthetic), then **Start round 2 with 2 shortlisted**.
2. As each bidder, submit a revised offer on **Your bid**: Harbor Capital Partners (synthetic) `20000000`, Northline Strategic (synthetic) `18000000` → **Submit revised offer**. Every version stays listed.
3. As the seller, click **Award to Harbor Capital Partners (synthetic)**.

**You should see:** "Awarded. Every other bidder has been declined and their access ended." Harbor Capital Partners (synthetic)'s **Your bid** says **Selected by the seller**; Northline Strategic (synthetic) can no longer open the pact. The **Team** tab and the audit log record every step.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 2040 revenue lines, one per unit rent charge per month | **Yes** — billing export step |
| `rent-roll.csv` | Rent roll at 30 September 2026 (96 rows) | **Yes** — industry data step |
| `delinquency.csv` | Delinquent balances at 30 September 2026 (5 rows) | **Yes** — industry data step |
| `unit-inspections.csv` | Unit-condition inspections with repair estimates (96 rows) | **Yes** — industry data step |
| `operating-statements-monthly.csv` | Operating statements by month, October 2006 to September 2026 (one row per line per month) (2400 rows) | **No** — it is already inside `documents/99-data-room-extracts.pdf`, which you upload |
| `pnl.csv` | Operating statement by fiscal year (October to September), FY2007 to FY2026 (10 lines) | **Yes** — P&L step |
| `occupancy-history.csv` | Occupancy and average in-place rent by month, October 2006 to September 2026 (240 rows) | **Yes** — industry data step |
| `rent-roll-history.csv` | Rent-roll snapshots at each quarter end, December 2024 to September 2026 (768 rows) | **Yes** — industry data step |
| `t12.csv` | Trailing-twelve-month operating statement (T-12) (12 rows) | **Yes** — industry data step |
| `documents/01-offering-memorandum.pdf` | Offering memorandum with stated NOI and capital plan | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `bidders.csv` | The three bidding firms for Part B: who to invite, what each asks and offers | **No** — read it while you follow Part B |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Notes

- Residents are referred to by unit only; there are no personal names.
- The rent roll maps onto the billing import: each occupied unit is a customer billed monthly.
- History (T-183): five fiscal years, October to September, FY2022 to FY2026; FY2026 is the T-12, so `t12.csv` equals the last twelve months of `operating-statements-monthly.csv` and of `pnl.csv`'s FY2026 column, and the September 2026 month of `occupancy-history.csv` matches `rent-roll.csv`.
- Figures the history checks reproduce: NOI growth -0.1% a year and revenue growth 1.4% a year (FY2022–FY2026); average in-place rent FY2022 USD 1,527.25, FY2023 USD 1,576.12, FY2024 USD 1,626.56, FY2025 USD 1,678.61, FY2026 USD 1,732.32 (3.2% a year); occupancy FY2022 95.3%, FY2023 95.1%, FY2024 93.1%, FY2025 91.2%, FY2026 88.5%; expense ratio 45.4% in FY2026; trailing three-year vacancy 9.1%.
- `operating-statements-monthly.csv` is the same statement as a long file (one row per line per month); it imports through the same P&L import. `rent-roll-history.csv` holds quarterly rent-roll snapshots for the last two years.
- Twenty years (T-185): `pnl.csv`, `operating-statements-monthly.csv` and `occupancy-history.csv` run back to FY2007 (October 2006). Planted: a 2009 downturn (occupancy and rents fall, the margin compresses) with a multi-year recovery, and a recent run above the long-run average. The five-year figures above are unchanged: the trend checks read the latest five years.
- Long-run figures the history checks reproduce: revenue growth 2.2% a year over ten years (FY2017–FY2026) and 1.8% over the full history; NOI growth 4.2% and 3.0%; revenue's worst year FY2009, down 12.6%, recovered to the FY2008 peak in FY2014 (5 years); NOI's worst year FY2009, down 30.1%, recovered to the FY2008 peak in FY2014 (5 years); occupancy's worst year FY2009, down 6.8 points, recovered to the FY2007 peak in FY2018 (9 years); NOI margin through the cycle 46.4% (last five years 55.3%); occupancy through the cycle 91.1% (last five years 92.6%).

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
| `02 Finance/Exports/Larkfield delinquency report export Sep26.csv` | Delinquency report |  |
| `02 Finance/Exports/Larkfield invoice lines export Sep26.csv` | Invoice lines |  |
| `02 Finance/Exports/Larkfield occupancy and rent history export Sep26.csv` | Occupancy and rent history |  |
| `02 Finance/Exports/Larkfield profit and loss (p&l) export Sep26.csv` | Profit and loss (P&L) |  |
| `02 Finance/Exports/Larkfield rent roll export Sep26.csv` | Rent roll |  |
| `02 Finance/Exports/Larkfield rent roll snapshots export Sep26.csv` | Rent roll snapshots |  |
| `02 Finance/Exports/Larkfield t-12 operating statement export Sep26.csv` | T-12 operating statement |  |
| `02 Finance/Larkfield FY26 summary.md` | Pactlab asks: income statement or cash flow statement? | Mixes profit and cash flow lines. |
| `02 Finance/Mgmt accounts FY26 - Larkfield.md` | Income statement (P&L) | Revenue matches the invoice lines for Oct 2025 – Sep 2026. |
| `02 Finance/Offering memorandum.pdf` | Other |  |

**And on the Intake checklist**, these should show as missing: **Cash flow statement**, **Unit inspections**.
Once billing is imported, **Customer contract** shows **Some missing** and names the largest billed customers with no contract in the room.
Click **Ask the seller** (or **Copy request for missing items**) to send the list.
