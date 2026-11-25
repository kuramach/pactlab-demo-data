# Cinder Ridge Energy B.V. — Energy generation and rights (EUR)

**Fictional target.** Cinder Ridge Energy B.V. sells a 600 MW coal-fired plant, Cinder Ridge Station (synthetic), together with a portfolio of oil and gas mineral, royalty and working interests in 20 wells.
Based in Utrecht, the Netherlands; reports in EUR. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Before you start

- Download this whole folder (on GitHub: **Code → Download ZIP** at the top of the repository, then unzip).
- Sign in to Pactlab. The steps take about 15 minutes.
- You upload **6 CSV files** and **8 PDFs**. Nothing else.
- **Never upload the `.md` files** in `documents/`. They are the text each PDF is built from; Pactlab reads the PDFs.
- `vdr-index.csv` is for reference only (how a data room would list these files). Do not upload it.
- Text in **bold** below is a button, tab or option exactly as Pactlab shows it.

## Two ways to test this company

- **Part A — Buyer side** (Steps 1 onwards): you are a buyer doing diligence on Cinder Ridge Energy B.V..
- **Part B — Seller side** ([below](#part-b--seller-side-run-a-bid-process)): you are Cinder Ridge Energy B.V., inviting several buyers — they ask questions, then offer or pass, and you choose one. Uses `bidders.csv`.
- Each part starts its own Pact, so you can do either one, or both.

# Part A — Buyer side

## Step 1 — Start the Pact

1. Click **Start a Pact** (top right).
2. **Name the Pact** — Pact name: `Project Cinder` · Base currency: **EUR** → **Next**.
3. **Buying entity** — Legal or trading name: `Demo Buyer` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `Cinder Ridge Energy B.V.` · **Private** · What kind of company is it?: **Energy generation & rights** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `170000000` (EUR 170,000,000) |
   | Currency | **EUR** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the seller's ask for the plant and the interests together. The demo shows how far the evidence supports it.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `Cinder Ridge Energy B.V.`, with the asking price EUR 170,000,000.

## Step 2 — Upload the billing export

1. Open the **Sources** tab → **Upload billing export**.
2. *1. Where is the export from?* → **Pactlab standard template**.
3. *2. Choose the file* → `invoice-lines.csv` → **Upload and map columns**.
4. The columns are matched for you. Click **Check every row**, then **Import 48 lines**.

**You should see:** a green message ending "Finances now include them." The **Finances** tab now shows the revenue ledger.

## Step 3 — Upload the industry data

Open the **Sources** tab and scroll to **Industry data**. Upload these files one at a time:

| # | Click | Choose the file | Then | Button should read |
|---|---|---|---|---|
| 1 | **Upload plant register** | `plant-register.csv` | **Upload and map columns** → **Check every row** | **Import 1 rows** |
| 2 | **Upload interest register** | `interest-register.csv` | **Upload and map columns** → **Check every row** | **Import 20 rows** |
| 3 | **Upload lease schedule** | `lease-schedule.csv` | **Upload and map columns** → **Check every row** | **Import 26 rows** |
| 4 | **Upload production history** | `production-history.csv` | **Upload and map columns** → **Check every row** | **Import 1008 rows** |
| 5 | **Upload liability schedule** | `liability-schedule.csv` | **Upload and map columns** → **Check every row** | **Import 7 rows** |

**You should see** after each import: "… imported … Industry checks ran on them". Some findings may already appear as drafts; that is expected.

## Step 4 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/01-sale-summary.pdf` | **business information** | The seller's sale summary |
| 2 | `documents/02-title-opinion.pdf` | **business information** | Division-order title opinion over the interests |
| 3 | `documents/03-division-order-og007.pdf` | **business information** | The operator's division order for one well |
| 4 | `documents/04-power-purchase-agreement.pdf` | **business information** | The plant's power purchase agreement |
| 5 | `documents/05-reserve-report.pdf` | **business information** | Third-party reserve report: reserves by category, values and the decline assumed |
| 6 | `documents/06-ash-pond-closure-plan.pdf` | **business information** | Closure and remediation plan for the plant's coal ash pond |
| 7 | `documents/07-decommissioning-study.pdf` | **business information** | Decommissioning study for the plant |
| 8 | `documents/99-data-room-extracts.pdf` | **financial information** | Every CSV extract in this folder as one paged PDF, so findings can cite a page |

**You should see:** all 8 documents listed on the **Documents** tab.

## Step 5 — Read the reserves and liabilities (Assets tab)

Open the **Assets** tab (it appears only on an energy generation & rights pact).

**You should see:** the plant and the 20 interests, contract coverage of about 80% on the plant, production declining about 10% a year, **Lease expiry**: 25.0% of the net acres not held by production inside the 5-year hold, one **division-order decimal** off the lease chain, and the **Liabilities** table: the ash pond unbooked and the ARO 40% short.

1. Under **Read the reports**, click **Read with AI** for `05-reserve-report.pdf`, `06-ash-pond-closure-plan.pdf` and `07-decommissioning-study.pdf`.
2. Under **To confirm**, check each proposed entry against its quote, then **Confirm** it (or correct it first, or **Reject** it). Only confirmed entries count: the reserves appear under **Reserves** as the report states them.
3. Click **Run energy checks**: it runs the same rules as Findings, over the confirmed entries too, and adds nothing already drafted.

## Step 6 — Run the checks and review the findings

1. Open the **Findings** tab → **Run energy generation & rights checks**.
2. **You should see exactly these 5 findings** (running the checks again adds nothing):

   1. **Unbooked environmental liability: Coal ash (CCR) closure at Cinder Ridge Station (synthetic)** — planted defect (a): `documents/06-ash-pond-closure-plan.pdf` page 2 estimates EUR 16,928,000; `liability-schedule.csv` books nothing for the ash pond. A remediation cost.
   2. **ARO shortfall: Cinder Ridge Station (synthetic)** — planted defect (b): the decommissioning study estimates EUR 38,640,000; the schedule books EUR 23,184,000 (60%), EUR 15,456,000 short — underfunded by 40%. An escrow.
   3. **Lease expiry risk: acreage not held by production** — planted defect (c): 25.0% of the net acres (1300 of 5200) are not held by production and expire by 31 March 2028, within 18 months.
   4. **Royalty decimal error: Blackjack 7H (synthetic)** — planted defect (d): the division order for OG-007 pays 0.12500000; the lease chain (0.5 × 3/16) supports 0.09375000 — overpaid by about EUR 42,424 a year.
   5. **PPA cliff: Cinder Ridge Station (synthetic)** — the PPA with Valley Electric Cooperative (synthetic) ends on 2028-06-30, inside the 5-year hold: 80% of the plant's revenue turns merchant.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 7 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

# Part B — Seller side: run a bid process

Here you are Cinder Ridge Energy B.V. You invite three bidders from `bidders.csv`, share a little, answer their questions and choose one.
Each bidder sees only their own bid — never another bidder's questions, offers or whether they passed. Part B checks that too.

**Addresses.** This folder holds no email addresses. Invite **an address you can read for each firm**: your own address with `+` and the firm's tag from `bidders.csv` added before the @ (for tag `harbor`: *yourname+harbor* at your email domain — Gmail, Outlook and most providers deliver it to you). On your own computer (`pnpm dev`) any made-up address works: every email Pactlab sends, invitations and sign-in codes, is written to `apps/api/.data/mail/`.

## Step B1 — Start the Pact as the seller

1. Click **Start a Pact** (top right).
2. Under *Who are you in this deal?* choose **We are selling (or raising)**. Pact name: `Project Cinder Sale` · Base currency: **EUR** → **Next**. (There is no buying-entity step.)
3. **Selling entity** — Legal or trading name: `Cinder Ridge Energy B.V.` · **Private** · What kind of company is it?: **Energy generation & rights** → **Next**.
4. **Asking price** — enter the same asking price as Part A, Step 1 (`170000000`) → **Next**.
5. **Review and start** — the Buyer box says *Bid process — you invite buyers once the pact starts* → **Start Pact**.

**You should see:** the **Bidders** page, with no bidders yet.

## Step B2 — Decide what bidders see

On **Bidders**, under **What bidders see**:

| Field | Enter |
|---|---|
| Shared summary | `Cinder Ridge Energy B.V. sells a 600 MW coal-fired plant, Cinder Ridge Station (synthetic), together with a portfolio of oil and gas mineral, royalty and working interests in 20 wells.` |
| Your data room (link) | `https://dataroom.example/energy-generation` (Pactlab is not the data room; this is where you would grant access) |
| NDA | `Mutual NDA (synthetic): everything shared about Cinder Ridge Energy B.V. stays confidential.` |
| Offer deadline (UTC) | a date a week from today |

→ **Save**.

Then open the **Documents** tab and upload `documents/01-sale-summary.pdf` with **Share with bidders** ticked (it is chosen at upload and cannot be changed later). Upload nothing else as shared — the rest stays with you.

**You should see:** "Saved. Bidders see the shared view once they accept the NDA." On Documents, `01-sale-summary.pdf` is listed.

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
   | Price | `160000000` (EUR 160,000,000) |
   | Currency | `EUR` |
   | Structure (cash, shares, earn-out…) | `Cash at close for 100% of the shares` |
   | Conditions | `Subject to confirmatory diligence and committed financing` |

   → **Submit offer**.
3. **Northline Strategic (synthetic)**: ask `Can you share the last three years of audited accounts?` → **Ask**. Then offer **Price** `140000000` (EUR 140,000,000), **Structure** `80% cash at close, 20% earn-out over 24 months`, **Conditions** `Key-person retention for the founders` → **Submit offer**.
4. **Atlas Growth Equity (synthetic)**: accept the NDA, then type `Outside our sector focus this year.` as the reason → **Pass on this pact**.

**You should see**, as Northline Strategic (synthetic): your own question and offer only — nothing of Harbor Capital Partners (synthetic)'s question or offer, and no sign that Atlas Growth Equity (synthetic) passed. There are no deal tabs; trying `/deals/<id>/bidders` shows nothing of the seller's side.

## Step B5 — Answer the questions

Back as the seller (your normal window), on **Bidders** under **Questions from bidders**:

- Harbor Capital Partners (synthetic)'s question → answer `One customer contract has a change-of-control clause; it is in the shared documents.` → choose **All bidders (without naming who asked)** → **Answer**.
- Northline Strategic (synthetic)'s question → answer `FY2024 and FY2025 are audited; FY2026 closes in December. We will add them to the data room.` → keep **Only Northline Strategic (synthetic)** → **Answer**.

**You should see**, as Northline Strategic (synthetic) (refresh **Your bid**): your private answer, and under *Answered to all bidders* the change-of-control question — without the name of who asked it. Harbor Capital Partners (synthetic) sees the answer to all, but not Northline Strategic (synthetic)'s private one.

## Step B6 — Compare the offers

On **Bidders**, **Offers side by side** sets the two offers next to each other — price, structure, conditions, version. Pactlab does not rank them or recommend one.

**You should see:** Harbor Capital Partners (synthetic) at EUR 160,000,000 and Northline Strategic (synthetic) at EUR 140,000,000; Atlas Growth Equity (synthetic) marked **Passed** with its reason.

## Step B7 — Shortlist, run round 2 and choose

1. Click **Shortlist** on Harbor Capital Partners (synthetic) and on Northline Strategic (synthetic), then **Start round 2 with 2 shortlisted**.
2. As each bidder, submit a revised offer on **Your bid**: Harbor Capital Partners (synthetic) `160000000`, Northline Strategic (synthetic) `150000000` → **Submit revised offer**. Every version stays listed.
3. As the seller, click **Award to Harbor Capital Partners (synthetic)**.

**You should see:** "Awarded. Every other bidder has been declined and their access ended." Harbor Capital Partners (synthetic)'s **Your bid** says **Selected by the seller**; Northline Strategic (synthetic) can no longer open the pact. The **Team** tab and the audit log record every step.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 48 revenue lines, one per power sale per month | **Yes** — billing export step |
| `plant-register.csv` | Plant register: capacity, fuel, age, capacity factor and PPA (1 rows) | **Yes** — industry data step |
| `interest-register.csv` | Interest register: mineral, royalty and working interests with the division-order decimal (20 rows) | **Yes** — industry data step |
| `lease-schedule.csv` | Lease schedule: net acres, royalty chain, primary term and whether production holds each lease (26 rows) | **Yes** — industry data step |
| `production-history.csv` | Production history: plant generation and revenue by contract type, and well volumes and gross revenue (1008 rows) | **Yes** — industry data step |
| `liability-schedule.csv` | The seller's liability schedule: environmental and retirement obligations as booked (7 rows) | **Yes** — industry data step |
| `documents/01-sale-summary.pdf` | The seller's sale summary | **Yes** — documents step |
| `documents/02-title-opinion.pdf` | Division-order title opinion over the interests | **Yes** — documents step |
| `documents/03-division-order-og007.pdf` | The operator's division order for one well | **Yes** — documents step |
| `documents/04-power-purchase-agreement.pdf` | The plant's power purchase agreement | **Yes** — documents step |
| `documents/05-reserve-report.pdf` | Third-party reserve report: reserves by category, values and the decline assumed | **Yes** — documents step |
| `documents/06-ash-pond-closure-plan.pdf` | Closure and remediation plan for the plant's coal ash pond | **Yes** — documents step |
| `documents/07-decommissioning-study.pdf` | Decommissioning study for the plant | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `bidders.csv` | The three bidding firms for Part B: who to invite, what each asks and offers | **No** — read it while you follow Part B |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Notes

- Buyer-side pack: you are buying the plant and the interests. Registers, the lease schedule, production and the liability schedule are CSV imports; the reserve report and environmental reports are read on the **Assets** tab, where a person confirms each entry before it counts.
- For the **Valuation** tab: **Reserve-based DCF** for the interests (the reserve report's categories and values on the **Assets** tab), or **Capacity value ($/kW)** for the plant — enter the net capacity in kW (600000) and a price per kW.
- Reserves are the third-party engineer's, cited as such; Pactlab never estimates reserves. A missing report is a gap finding.
- Diligence support only: not legal, engineering or regulatory advice. Pactlab makes no title determination and certifies no reserves.

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
| `02 Finance/Ash pond closure plan.pdf` | Other |  |
| `02 Finance/Cinder FY26 summary.md` | Pactlab asks: income statement or cash flow statement? | Mixes profit and cash flow lines. |
| `02 Finance/Decommissioning study.pdf` | Other |  |
| `02 Finance/Division order og007.pdf` | Other |  |
| `02 Finance/Exports/Cinder invoice lines export Sep26.csv` | Invoice lines |  |
| `02 Finance/Mgmt accounts FY26 - Cinder.md` | Income statement (P&L) | Revenue matches the invoice lines for Oct 2025 – Sep 2026. |
| `02 Finance/Reserve report.pdf` | Other |  |
| `02 Finance/Sale summary.pdf` | Other |  |
| `02 Finance/Title opinion.pdf` | Other |  |
| `03 Commercial/Customers/Power purchase agreement (signed copy).pdf` | Duplicate — shown once | Same bytes as the agreement above. |
| `03 Commercial/Customers/Power purchase agreement.pdf` | Customer contract |  |

**And on the Intake checklist**, these should show as missing: **Cash flow statement**.
Once billing is imported, **Customer contract** shows **Some missing** and names the largest billed customers with no contract in the room.
Click **Ask the seller** (or **Copy request for missing items**) to send the list.
