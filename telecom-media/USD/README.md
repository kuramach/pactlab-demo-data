# Northlake Fibre Inc. — Telecom and media (USD)

**Fictional target.** Northlake Fibre Inc. is a regional fibre broadband and streaming-TV provider selling residential and small-business plans in four regions, with a regional sports channel carried by other distributors.
Based in Columbus, Ohio, United States; reports in USD. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Before you start

- Download this whole folder (on GitHub: **Code → Download ZIP** at the top of the repository, then unzip).
- Sign in to Pactlab. The steps take about 15 minutes.
- You upload **6 CSV files** and **5 PDFs**. Nothing else.
- **Never upload the `.md` files** in `documents/`. They are the text each PDF is built from; Pactlab reads the PDFs.
- `vdr-index.csv` is for reference only (how a data room would list these files). Do not upload it.
- Text in **bold** below is a button, tab or option exactly as Pactlab shows it.

## Two ways to test this company

- **Part A — Buyer side** (Steps 1 onwards): you are a buyer doing diligence on Northlake Fibre Inc..
- **Part B — Seller side** ([below](#part-b--seller-side-run-a-bid-process)): you are Northlake Fibre Inc., inviting several buyers — they ask questions, then offer or pass, and you choose one. Uses `bidders.csv`.
- Each part starts its own Pact, so you can do either one, or both.

# Part A — Buyer side

## Step 1 — Start the Pact

1. Click **Start a Pact** (top right).
2. **Name the Pact** — Pact name: `Project Northlake` · Base currency: **USD** → **Next**.
3. **Buying entity** — Legal or trading name: `Demo Buyer` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `Northlake Fibre Inc.` · **Private** · What kind of company is it?: **Telecom & media** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `23000000` (USD 23,000,000) |
   | Currency | **USD** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the seller's ask: 3× the September 2026 billed revenue run-rate. The demo shows how far the evidence supports it.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `Northlake Fibre Inc.`, with the asking price USD 23,000,000.

## Step 2 — Upload the billing export

1. Open the **Sources** tab → **Upload billing export**.
2. *1. Where is the export from?* → **Pactlab standard template**.
3. *2. Choose the file* → `invoice-lines.csv` → **Upload and map columns**.
4. The columns are matched for you. Click **Check every row**, then **Import 288 lines**.

**You should see:** a green message ending "Finances now include them." The **Finances** tab now shows the revenue ledger.

## Step 3 — Upload the industry data

Open the **Sources** tab and scroll to **Industry data**. Upload these files one at a time:

| # | Click | Choose the file | Then | Button should read |
|---|---|---|---|---|
| 1 | **Upload subscribers by month** | `subscribers-by-month.csv` | **Upload and map columns** → **Check every row** | **Import 144 rows** |
| 2 | **Upload subscriber movements** | `subscriber-movements.csv` | **Upload and map columns** → **Check every row** | **Import 828 rows** |
| 3 | **Upload rights and carriage register** | `rights-register.csv` | **Upload and map columns** → **Check every row** | **Import 7 rows** |
| 4 | **Upload advertising and affiliate revenue** | `revenue-by-counterparty.csv` | **Upload and map columns** → **Check every row** | **Import 264 rows** |
| 5 | **Upload capital expenditure by year** | `capex-by-year.csv` | **Upload and map columns** → **Check every row** | **Import 20 rows** |

**You should see** after each import: "… imported … Industry checks ran on them". Some findings may already appear as drafts; that is expected.

## Step 4 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/01-kpi-pack-2026-09.pdf` | **business information** | Management KPI pack with reported subscribers and churn |
| 2 | `documents/02-wholesale-network-agreement.pdf` | **business information** | Wholesale network access agreement |
| 3 | `documents/03-investor-presentation.pdf` | **business information** | Investor presentation with the subscriber, churn and ARPU claims and the expected closing date |
| 4 | `documents/04-affiliation-agreement-rivermark.pdf` | **business information** | Affiliation agreement with Rivermark Cable, the largest distributor of the sports channel |
| 5 | `documents/99-data-room-extracts.pdf` | **financial information** | Every CSV extract in this folder as one paged PDF, so findings can cite a page |

**You should see:** all 5 documents listed on the **Documents** tab.

## Step 5 — Upload the P&L by year

Open the **Sources** tab, scroll to **Industry data** and click **Upload profit and loss (p&l)**.

1. Choose `pnl.csv` → **Upload and map columns**. Pactlab reads the five years across the columns (FY2021 to FY2025).
2. Say what each line is: the three lines ending in *revenue* are **Revenue**, the three lines starting *Cost of* are **Cost of revenue**, and the rest are **Operating expenses**.
3. **Check every row**, then **Import 40 rows**.

**You should see:** the import succeed. The **Subscribers** tab now shows the P&L year by year and content cost per subscriber against ARPU; **Finances** shows the five years side by side with subscribers, churn and ARPU, and the checks in the next step read every year.

## Step 6 — Run the checks and review the findings

1. Open the **Findings** tab → **Run telecom & media checks**.
2. **You should see exactly these 14 findings** (running the checks again adds nothing):

   1. **Reported subscribers exceed billed subscribers** — the KPI pack reports 12,382; `subscribers-by-month.csv` bills 11,638 in September 2026.
   2. **Churn rising against the reported rate** — billed subscribers grow about 0.3% a month until December 2025, then shrink about 0.5% a month from January 2026 (`invoice-lines.csv`, `subscribers-by-month.csv`); the KPI pack still reports 0.9% churn.
   3. **Regional concentration** — the North region is 44.7% of September 2026 revenue.
   4. **Wholesale price review ahead** — `documents/02-wholesale-network-agreement.pdf` page 2, clause 9 — next re-pricing 1 January 2027.
   5. **Claim verified: Subscribers** — the investor presentation says 11,638 billed subscribers; `subscriber-movements.csv` closes September 2026 at 11,638.
   6. **Claim contradicted: Monthly churn** — the investor presentation says 0.9% a month; `subscriber-movements.csv` gives 1.5% a month over the twelve months to September 2026 (disconnects ÷ opening subscribers).
   7. **Claim verified: ARPU** — the investor presentation says USD 54.12 a month; `subscriber-movements.csv` gives the same over the twelve months to September 2026.
   8. **Material agreement ends within 12 months of the closing: AF-01** — `documents/04-affiliation-agreement-rivermark.pdf` page 2 — AF-01 expires on 30 September 2027 and does not renew automatically, nine months after the 31 December 2026 closing (the register says 2028). It is 6.6% of trailing revenue.
   9. **Advertising revenue concentrated in one counterparty: Brightline Motors (synthetic)** — `revenue-by-counterparty.csv` — Brightline Motors is 34.0% of advertising revenue over the twelve months to September 2026.
   10. **Content costs rising against flat ARPU, 2021–2025** — `pnl.csv` and `subscriber-movements.csv` — content cost per subscriber a month 2021 13.51, 2022 15.17, 2023 16.83, 2024 20.59, 2025 24.33 against ARPU 2021 54.28, 2022 54.28, 2023 54.28, 2024 54.28, 2025 54.28. A single year shows only that year.
   11. **Monthly churn rising every year, FY2021–FY2025** — `subscriber-movements.csv` — disconnects ÷ opening subscribers by calendar year: FY2021 0.66%, FY2022 0.73%, FY2023 0.79%, FY2024 0.86%, FY2025 0.91%. The trailing twelve months alone do not show it.
   12. **P&L trend, 2021–2025** — every imported year side by side: revenue, growth, margins and the content, network, carriage and marketing ratios.
   13. **Gross margin and Operating margin down across 2021–2025** — `pnl.csv` — gross margin 59.0% to 46.0%, operating margin 44.0% to 31.0%.
   14. **Content and programming costs growing faster than revenue, 2021–2025** — `pnl.csv` — 16.0% of revenue in FY2021 to 29.0% in FY2025.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 7 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

# Part B — Seller side: run a bid process

Here you are Northlake Fibre Inc. You invite three bidders from `bidders.csv`, share a little, answer their questions and choose one.
Each bidder sees only their own bid — never another bidder's questions, offers or whether they passed. Part B checks that too.

**Addresses.** This folder holds no email addresses. Invite **an address you can read for each firm**: your own address with `+` and the firm's tag from `bidders.csv` added before the @ (for tag `harbor`: *yourname+harbor* at your email domain — Gmail, Outlook and most providers deliver it to you). On your own computer (`pnpm dev`) any made-up address works: every email Pactlab sends, invitations and sign-in codes, is written to `apps/api/.data/mail/`.

## Step B1 — Start the Pact as the seller

1. Click **Start a Pact** (top right).
2. Under *Who are you in this deal?* choose **We are selling (or raising)**. Pact name: `Project Northlake Sale` · Base currency: **USD** → **Next**. (There is no buying-entity step.)
3. **Selling entity** — Legal or trading name: `Northlake Fibre Inc.` · **Private** · What kind of company is it?: **Telecom & media** → **Next**.
4. **Asking price** — enter the same asking price as Part A, Step 1 (`23000000`) → **Next**.
5. **Review and start** — the Buyer box says *Bid process — you invite buyers once the pact starts* → **Start Pact**.

**You should see:** the **Bidders** page, with no bidders yet.

## Step B2 — Decide what bidders see

On **Bidders**, under **What bidders see**:

| Field | Enter |
|---|---|
| Shared summary | `Northlake Fibre Inc. is a regional fibre broadband and streaming-TV provider selling residential and small-business plans in four regions, with a regional sports channel carried by other distributors.` |
| Your data room (link) | `https://dataroom.example/telecom-media` (Pactlab is not the data room; this is where you would grant access) |
| NDA | `Mutual NDA (synthetic): everything shared about Northlake Fibre Inc. stays confidential.` |
| Offer deadline (UTC) | a date a week from today |

→ **Save**.

Then open the **Documents** tab and upload `documents/01-kpi-pack-2026-09.pdf` with **Share with bidders** ticked (it is chosen at upload and cannot be changed later). Upload nothing else as shared — the rest stays with you.

**You should see:** "Saved. Bidders see the shared view once they accept the NDA." On Documents, `01-kpi-pack-2026-09.pdf` is listed.

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
   | Price | `21000000` (USD 21,000,000) |
   | Currency | `USD` |
   | Structure (cash, shares, earn-out…) | `Cash at close for 100% of the shares` |
   | Conditions | `Subject to confirmatory diligence and committed financing` |

   → **Submit offer**.
3. **Northline Strategic (synthetic)**: ask `Can you share the last three years of audited accounts?` → **Ask**. Then offer **Price** `20000000` (USD 20,000,000), **Structure** `80% cash at close, 20% earn-out over 24 months`, **Conditions** `Key-person retention for the founders` → **Submit offer**.
4. **Atlas Growth Equity (synthetic)**: accept the NDA, then type `Outside our sector focus this year.` as the reason → **Pass on this pact**.

**You should see**, as Northline Strategic (synthetic): your own question and offer only — nothing of Harbor Capital Partners (synthetic)'s question or offer, and no sign that Atlas Growth Equity (synthetic) passed. There are no deal tabs; trying `/deals/<id>/bidders` shows nothing of the seller's side.

## Step B5 — Answer the questions

Back as the seller (your normal window), on **Bidders** under **Questions from bidders**:

- Harbor Capital Partners (synthetic)'s question → answer `One customer contract has a change-of-control clause; it is in the shared documents.` → choose **All bidders (without naming who asked)** → **Answer**.
- Northline Strategic (synthetic)'s question → answer `FY2024 and FY2025 are audited; FY2026 closes in December. We will add them to the data room.` → keep **Only Northline Strategic (synthetic)** → **Answer**.

**You should see**, as Northline Strategic (synthetic) (refresh **Your bid**): your private answer, and under *Answered to all bidders* the change-of-control question — without the name of who asked it. Harbor Capital Partners (synthetic) sees the answer to all, but not Northline Strategic (synthetic)'s private one.

## Step B6 — Compare the offers

On **Bidders**, **Offers side by side** sets the two offers next to each other — price, structure, conditions, version. Pactlab does not rank them or recommend one.

**You should see:** Harbor Capital Partners (synthetic) at USD 21,000,000 and Northline Strategic (synthetic) at USD 20,000,000; Atlas Growth Equity (synthetic) marked **Passed** with its reason.

## Step B7 — Shortlist, run round 2 and choose

1. Click **Shortlist** on Harbor Capital Partners (synthetic) and on Northline Strategic (synthetic), then **Start round 2 with 2 shortlisted**.
2. As each bidder, submit a revised offer on **Your bid**: Harbor Capital Partners (synthetic) `22000000`, Northline Strategic (synthetic) `20000000` → **Submit revised offer**. Every version stays listed.
3. As the seller, click **Award to Harbor Capital Partners (synthetic)**.

**You should see:** "Awarded. Every other bidder has been declined and their access ended." Harbor Capital Partners (synthetic)'s **Your bid** says **Selected by the seller**; Northline Strategic (synthetic) can no longer open the pact. The **Team** tab and the audit log record every step.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 288 revenue lines, one per region-and-plan subscriber billing per month | **Yes** — billing export step |
| `subscribers-by-month.csv` | Billed subscribers and ARPU by region and plan (144 rows) | **Yes** — industry data step |
| `subscriber-movements.csv` | Subscriber movements by month, region and plan from the billing system: opening, gross additions, disconnects, closing and service revenue (828 rows) | **Yes** — industry data step |
| `revenue-by-counterparty.csv` | Advertising and affiliate revenue by month and counterparty, from the ad-sales and affiliate statements (264 rows) | **Yes** — industry data step |
| `rights-register.csv` | Rights and carriage register: content, affiliate, carriage and sports-rights agreements with their annual value and dates (7 rows) | **Yes** — industry data step |
| `pnl.csv` | Profit and loss by fiscal year, FY2021 to FY2025 (8 lines) | **Yes** — P&L step |
| `capex-by-year.csv` | Capital expenditure by fiscal year and category, FY2021 to FY2025 (20 rows) | **Yes** — industry data step |
| `documents/01-kpi-pack-2026-09.pdf` | Management KPI pack with reported subscribers and churn | **Yes** — documents step |
| `documents/02-wholesale-network-agreement.pdf` | Wholesale network access agreement | **Yes** — documents step |
| `documents/03-investor-presentation.pdf` | Investor presentation with the subscriber, churn and ARPU claims and the expected closing date | **Yes** — documents step |
| `documents/04-affiliation-agreement-rivermark.pdf` | Affiliation agreement with Rivermark Cable, the largest distributor of the sports channel | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `bidders.csv` | The three bidding firms for Part B: who to invite, what each asks and offers | **No** — read it while you follow Part B |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Notes

- Subscribers appear only as counts by region and plan, never as people; advertisers and distributors are businesses.
- `subscriber-movements.csv` runs January 2021 to September 2026, so each of FY2021–FY2025 is a complete year (five years of history, read side by side on **Finances**); its service revenue ties to the P&L's subscription revenue year by year.
- The agreement governs over the register: `rights-register.csv` gives AF-01 an end of 2028-09-30, the agreement itself 30 September 2027.
- The P&L (`pnl.csv`) imports through Sources like any extract; the multi-year checks read every year it holds. A single year still imports: the trend then reports that year alone.

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
| `02 Finance/Exports/Northlake invoice lines export Sep26.csv` | Invoice lines |  |
| `02 Finance/Exports/Northlake subscribers by month export Sep26.csv` | Subscribers by month |  |
| `02 Finance/Investor presentation.pdf` | Other |  |
| `02 Finance/Kpi pack 2026 09.pdf` | Other |  |
| `02 Finance/Mgmt accounts FY26 - Northlake.md` | Income statement (P&L) | Revenue matches the invoice lines for Oct 2025 – Sep 2026. |
| `02 Finance/Northlake FY26 summary.md` | Pactlab asks: income statement or cash flow statement? | Mixes profit and cash flow lines. |
| `03 Commercial/Customers/Affiliation agreement rivermark (signed copy).pdf` | Duplicate — shown once | Same bytes as the agreement above. |
| `03 Commercial/Customers/Affiliation agreement rivermark.pdf` | Customer contract |  |
| `03 Commercial/Suppliers/Wholesale network agreement.pdf` | Supplier contract |  |

**And on the Intake checklist**, these should show as missing: **Cash flow statement**.
Once billing is imported, **Customer contract** shows **Some missing** and names the largest billed customers with no contract in the room.
Click **Ask the seller** (or **Copy request for missing items**) to send the list.
