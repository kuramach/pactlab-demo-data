# Ridgeline Outfitters Inc. — E-commerce and DTC (USD)

**Fictional target.** Ridgeline Outfitters Inc. sells outdoor apparel direct to consumers through its own store, one large marketplace and a few wholesale retailers.
Based in Columbus, Ohio, United States; reports in USD. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Before you start

- Download this whole folder (on GitHub: **Code → Download ZIP** at the top of the repository, then unzip).
- Sign in to Pactlab. The steps take about 15 minutes.
- You upload **5 CSV files** and **4 PDFs**. Nothing else.
- **Never upload the `.md` files** in `documents/`. They are the text each PDF is built from; Pactlab reads the PDFs.
- `vdr-index.csv` is for reference only (how a data room would list these files). Do not upload it.
- Text in **bold** below is a button, tab or option exactly as Pactlab shows it.

## Two ways to test this company

- **Part A — Buyer side** (Steps 1 onwards): you are a buyer doing diligence on Ridgeline Outfitters Inc..
- **Part B — Seller side** ([below](#part-b--seller-side-run-a-bid-process)): you are Ridgeline Outfitters Inc., inviting several buyers — they ask questions, then offer or pass, and you choose one. Uses `bidders.csv`.
- Each part starts its own Pact, so you can do either one, or both.

# Part A — Buyer side

## Step 1 — Start the Pact

1. Click **Start a Pact** (top right).
2. **Name the Pact** — Pact name: `Project Ridgeline` · Base currency: **USD** → **Next**.
3. **Buying entity** — Legal or trading name: `Demo Buyer` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `Ridgeline Outfitters Inc.` · **Private** · What kind of company is it?: **E-commerce & DTC** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `4600000` (USD 4,600,000) |
   | Currency | **USD** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the seller's ask: 1.5× the September 2026 billed revenue run-rate. The demo shows how far the evidence supports it.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `Ridgeline Outfitters Inc.`, with the asking price USD 4,600,000.

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
| 1 | **Upload orders by cohort** | `orders-by-cohort.csv` | **Upload and map columns** → **Check every row** | **Import 69 rows** |
| 2 | **Upload ad spend** | `ad-spend.csv` | **Upload and map columns** → **Check every row** | **Import 24 rows** |
| 3 | **Upload orders by channel** | `channel-orders.csv` | **Upload and map columns** → **Check every row** | **Import 276 rows** |
| 4 | **Upload stock report** | `inventory.csv` | **Upload and map columns** → **Check every row** | **Import 36 rows** |

**You should see** after each import: "… imported … Industry checks ran on them". Some findings may already appear as drafts; that is expected.

## Step 4 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/01-marketplace-seller-terms.pdf` | **business information** | Marketplace seller terms |
| 2 | `documents/02-platform-accounts.pdf` | **business information** | Schedule of storefront, marketplace and ad accounts and who each is registered to |
| 3 | `documents/03-investor-presentation.pdf` | **business information** | Investor presentation with lifetime-value and acquisition-cost claims |
| 4 | `documents/99-data-room-extracts.pdf` | **financial information** | Every CSV extract in this folder as one paged PDF, so findings can cite a page |

**You should see:** all 4 documents listed on the **Documents** tab.

## Step 5 — Upload the P&L by year

Open the **Sources** tab, scroll to **Industry data** and click **Upload profit and loss (p&l)**.

1. Choose `pnl.csv` → **Upload and map columns**. Pactlab reads the five years across the columns (FY2021 to FY2025).
2. Say what each line is: the three lines ending in *revenue* are **Revenue**, the three lines starting *Cost of* are **Cost of revenue**, and the rest are **Operating expenses**.
3. **Check every row**, then **Import 45 rows**.

**You should see:** the import succeed. The **Channels** tab now shows the P&L year by year, reconciled to the channel exports; **Finances** shows the five years side by side with orders, order value, repeat rate and the discount rate, and the checks in the next step read every year.

## Step 6 — Run the checks and review the findings

1. Open the **Findings** tab → **Run e-commerce & dtc checks**.
2. **You should see exactly these 13 findings** (running the checks again adds nothing):

   1. **Majority of revenue through one marketplace** — Marketvale marketplace (synthetic) is 64.2% of September 2026 revenue.
   2. **Repeat purchase declining in recent cohorts** — `orders-by-cohort.csv` — cohorts from 2025-07 keep about 27% of customers in their second month, against about 39% for earlier cohorts.
   3. **Acquisition cost rising on paid social** — `ad-spend.csv` — paid-social spend rises every month while new customers fall.
   4. **Claim contradicted: Customer lifetime value** — the investor presentation states a 12-month LTV of USD 290; on a contribution-margin basis the exports give USD 77.58 (3.70 orders per customer × USD 20.96 contribution per order). The stated figure is the same orders valued at gross sales (USD 289.75).
   5. **Claim verified: Paid customer acquisition cost** — USD 40.97: ad spend ÷ attributed new customers, `ad-spend.csv`, twelve months to September 2026.
   6. **Platform account held personally: Marketvale marketplace (MV-20417)** — 64.0% of net sales in the twelve months to September 2026 ran through it (`channel-orders.csv`); `documents/02-platform-accounts.pdf` says it is registered to the founder personally.
   7. **Aged inventory: 22.0% of stock older than 180 days** — `inventory.csv` — USD 173,664 of USD 789,357 at landed cost was received more than 180 days before 30 September 2026; priced as a write-down.
   8. **Acquisition cost rising every year, 2021–2025** — blended CAC — advertising (`pnl.csv`) ÷ new customers (`channel-orders.csv`) — 2021 USD 13.01, 2022 USD 17.59, 2023 USD 23.01, 2024 USD 30.49, 2025 USD 39.76. A single year looks unremarkable.
   9. **Contribution margin compressing every year, 2021–2025** — `channel-orders.csv` — consumer contribution margin 2021 41.7%, 2022 40.0%, 2023 38.3%, 2024 35.3%, 2025 32.5%.
   10. **Discount rate rising every year, FY2021–FY2025** — `channel-orders.csv` — discounts ÷ gross sales by calendar year: FY2021 3.5%, FY2022 4.2%, FY2023 5.0%, FY2024 6.0%, FY2025 7.0%; growth is being bought with discounts.
   11. **P&L trend, 2021–2025** — every imported year side by side: revenue, growth, margins and the advertising, fulfilment and fee ratios.
   12. **Gross margin and Operating margin down across 2021–2025** — `pnl.csv` — gross margin 43.7% to 34.8%, operating margin 19.7% to 1.8%.
   13. **Advertising and marketing growing faster than revenue, 2021–2025** — `pnl.csv` — 8.0% of revenue in FY2021 to 17.0% in FY2025.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 7 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

# Part B — Seller side: run a bid process

Here you are Ridgeline Outfitters Inc. You invite three bidders from `bidders.csv`, share a little, answer their questions and choose one.
Each bidder sees only their own bid — never another bidder's questions, offers or whether they passed. Part B checks that too.

**Addresses.** This folder holds no email addresses. Invite **an address you can read for each firm**: your own address with `+` and the firm's tag from `bidders.csv` added before the @ (for tag `harbor`: *yourname+harbor* at your email domain — Gmail, Outlook and most providers deliver it to you). On your own computer (`pnpm dev`) any made-up address works: every email Pactlab sends, invitations and sign-in codes, is written to `apps/api/.data/mail/`.

## Step B1 — Start the Pact as the seller

1. Click **Start a Pact** (top right).
2. Under *Who are you in this deal?* choose **We are selling (or raising)**. Pact name: `Project Ridgeline Sale` · Base currency: **USD** → **Next**. (There is no buying-entity step.)
3. **Selling entity** — Legal or trading name: `Ridgeline Outfitters Inc.` · **Private** · What kind of company is it?: **E-commerce & DTC** → **Next**.
4. **Asking price** — enter the same asking price as Part A, Step 1 (`4600000`) → **Next**.
5. **Review and start** — the Buyer box says *Bid process — you invite buyers once the pact starts* → **Start Pact**.

**You should see:** the **Bidders** page, with no bidders yet.

## Step B2 — Decide what bidders see

On **Bidders**, under **What bidders see**:

| Field | Enter |
|---|---|
| Shared summary | `Ridgeline Outfitters Inc. sells outdoor apparel direct to consumers through its own store, one large marketplace and a few wholesale retailers.` |
| Your data room (link) | `https://dataroom.example/ecommerce-dtc` (Pactlab is not the data room; this is where you would grant access) |
| NDA | `Mutual NDA (synthetic): everything shared about Ridgeline Outfitters Inc. stays confidential.` |
| Offer deadline (UTC) | a date a week from today |

→ **Save**.

Then open the **Documents** tab and upload `documents/01-marketplace-seller-terms.pdf` with **Share with bidders** ticked (it is chosen at upload and cannot be changed later). Upload nothing else as shared — the rest stays with you.

**You should see:** "Saved. Bidders see the shared view once they accept the NDA." On Documents, `01-marketplace-seller-terms.pdf` is listed.

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
   | Price | `4200000` (USD 4,200,000) |
   | Currency | `USD` |
   | Structure (cash, shares, earn-out…) | `Cash at close for 100% of the shares` |
   | Conditions | `Subject to confirmatory diligence and committed financing` |

   → **Submit offer**.
3. **Northline Strategic (synthetic)**: ask `Can you share the last three years of audited accounts?` → **Ask**. Then offer **Price** `3900000` (USD 3,900,000), **Structure** `80% cash at close, 20% earn-out over 24 months`, **Conditions** `Key-person retention for the founders` → **Submit offer**.
4. **Atlas Growth Equity (synthetic)**: accept the NDA, then type `Outside our sector focus this year.` as the reason → **Pass on this pact**.

**You should see**, as Northline Strategic (synthetic): your own question and offer only — nothing of Harbor Capital Partners (synthetic)'s question or offer, and no sign that Atlas Growth Equity (synthetic) passed. There are no deal tabs; trying `/deals/<id>/bidders` shows nothing of the seller's side.

## Step B5 — Answer the questions

Back as the seller (your normal window), on **Bidders** under **Questions from bidders**:

- Harbor Capital Partners (synthetic)'s question → answer `One customer contract has a change-of-control clause; it is in the shared documents.` → choose **All bidders (without naming who asked)** → **Answer**.
- Northline Strategic (synthetic)'s question → answer `FY2024 and FY2025 are audited; FY2026 closes in December. We will add them to the data room.` → keep **Only Northline Strategic (synthetic)** → **Answer**.

**You should see**, as Northline Strategic (synthetic) (refresh **Your bid**): your private answer, and under *Answered to all bidders* the change-of-control question — without the name of who asked it. Harbor Capital Partners (synthetic) sees the answer to all, but not Northline Strategic (synthetic)'s private one.

## Step B6 — Compare the offers

On **Bidders**, **Offers side by side** sets the two offers next to each other — price, structure, conditions, version. Pactlab does not rank them or recommend one.

**You should see:** Harbor Capital Partners (synthetic) at USD 4,200,000 and Northline Strategic (synthetic) at USD 3,900,000; Atlas Growth Equity (synthetic) marked **Passed** with its reason.

## Step B7 — Shortlist, run round 2 and choose

1. Click **Shortlist** on Harbor Capital Partners (synthetic) and on Northline Strategic (synthetic), then **Start round 2 with 2 shortlisted**.
2. As each bidder, submit a revised offer on **Your bid**: Harbor Capital Partners (synthetic) `4500000`, Northline Strategic (synthetic) `4000000` → **Submit revised offer**. Every version stays listed.
3. As the seller, click **Award to Harbor Capital Partners (synthetic)**.

**You should see:** "Awarded. Every other bidder has been declined and their access ended." Harbor Capital Partners (synthetic)'s **Your bid** says **Selected by the seller**; Northline Strategic (synthetic) can no longer open the pact. The **Team** tab and the audit log record every step.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 96 revenue lines, one per sales-channel payout per month | **Yes** — billing export step |
| `channel-orders.csv` | Storefront and marketplace orders by month, channel and platform account, January 2021 to September 2026: sales, returns, costs and new customers (276 rows) | **Yes** — industry data step |
| `orders-by-cohort.csv` | Repeat purchase by first-purchase cohort (69 rows) | **Yes** — industry data step |
| `ad-spend.csv` | Advertising spend and new customers by channel (24 rows) | **Yes** — industry data step |
| `inventory.csv` | Stock report at 30 September 2026: units, landed cost and date received by SKU and location (36 rows) | **Yes** — industry data step |
| `pnl.csv` | Profit and loss by fiscal year, FY2021 to FY2025 (9 lines) | **Yes** — P&L step |
| `documents/01-marketplace-seller-terms.pdf` | Marketplace seller terms | **Yes** — documents step |
| `documents/02-platform-accounts.pdf` | Schedule of storefront, marketplace and ad accounts and who each is registered to | **Yes** — documents step |
| `documents/03-investor-presentation.pdf` | Investor presentation with lifetime-value and acquisition-cost claims | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `bidders.csv` | The three bidding firms for Part B: who to invite, what each asks and offers | **No** — read it while you follow Part B |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Notes

- `channel-orders.csv` runs January 2021 to September 2026, so each of FY2021–FY2025 is a complete year (five years of history, read side by side on **Finances**); the channel revenue in it ties to the P&L year by year.
- The P&L (`pnl.csv`) imports through Sources like any extract; the multi-year checks read every year it holds. A single year still imports: the trend then reports that year alone.
- Pactlab reads exports and documents only: it never logs in to the marketplace, storefront or ad platforms.

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
| `02 Finance/Exports/Ridgeline ad spend export Sep26.csv` | Ad spend |  |
| `02 Finance/Exports/Ridgeline invoice lines export Sep26.csv` | Invoice lines |  |
| `02 Finance/Investor presentation.pdf` | Other |  |
| `02 Finance/Marketplace seller terms.pdf` | Other |  |
| `02 Finance/Mgmt accounts FY26 - Ridgeline.md` | Income statement (P&L) | Revenue matches the invoice lines for Oct 2025 – Sep 2026. |
| `02 Finance/Platform accounts.pdf` | Other |  |
| `02 Finance/Ridgeline FY26 summary.md` | Pactlab asks: income statement or cash flow statement? | Mixes profit and cash flow lines. |

**And on the Intake checklist**, these should show as missing: **Cash flow statement**, **Orders by cohort**.
Once billing is imported, **Customer contract** shows **Some missing** and names the largest billed customers with no contract in the room.
Click **Ask the seller** (or **Copy request for missing items**) to send the list.
