# Riverside Care Partners B.V. — Healthcare services and healthtech (EUR)

**Fictional target.** Riverside Care Partners B.V. operates nine physical-therapy and primary-care practices, paid mostly by government programmes and commercial insurers.
Based in Utrecht, the Netherlands; reports in EUR. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Before you start

- Download this whole folder (on GitHub: **Code → Download ZIP** at the top of the repository, then unzip).
- Sign in to Pactlab. The steps take about 15 minutes.
- You upload **3 CSV files** and **3 PDFs**. Nothing else.
- **Never upload the `.md` files** in `documents/`. They are the text each PDF is built from; Pactlab reads the PDFs.
- `vdr-index.csv` is for reference only (how a data room would list these files). Do not upload it.
- Text in **bold** below is a button, tab or option exactly as Pactlab shows it.

## Two ways to test this company

- **Part A — Buyer side** (Steps 1 onwards): you are a buyer doing diligence on Riverside Care Partners B.V..
- **Part B — Seller side** ([below](#part-b--seller-side-run-a-bid-process)): you are Riverside Care Partners B.V., inviting several buyers — they ask questions, then offer or pass, and you choose one. Uses `bidders.csv`.
- Each part starts its own Pact, so you can do either one, or both.

# Part A — Buyer side

## Step 1 — Start the Pact

1. Click **Start a Pact** (top right).
2. **Name the Pact** — Pact name: `Project Riverside` · Base currency: **EUR** → **Next**.
3. **Buying entity** — Legal or trading name: `Demo Buyer` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `Riverside Care Partners B.V.` · **Private** · What kind of company is it?: **Healthcare & health tech** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `2200000` (EUR 2,200,000) |
   | Currency | **EUR** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the seller's ask: 1.5× the September 2026 billed revenue run-rate. The demo shows how far the evidence supports it.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `Riverside Care Partners B.V.`, with the asking price EUR 2,200,000.

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

   1. **Revenue concentrated in government programmes** — government programmes A and B are 64.2% of September 2026 revenue in `invoice-lines.csv`.
   2. **Medical-director fee above documented duties** — `documents/01-medical-director-agreement.pdf` — a fixed fee for four hours a month, against 1.5 documented hours (page 2).
   3. **Privacy risk assessment out of date** — `documents/02-privacy-risk-assessment.pdf` — last assessed March 2023, review overdue since March 2024.
   4. **Provider credentials expiring** — two providers in `provider-roster.csv` have credentials expiring before the end of 2026.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 6 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

# Part B — Seller side: run a bid process

Here you are Riverside Care Partners B.V. You invite three bidders from `bidders.csv`, share a little, answer their questions and choose one.
Each bidder sees only their own bid — never another bidder's questions, offers or whether they passed. Part B checks that too.

**Addresses.** This folder holds no email addresses. Invite **an address you can read for each firm**: your own address with `+` and the firm's tag from `bidders.csv` added before the @ (for tag `harbor`: *yourname+harbor* at your email domain — Gmail, Outlook and most providers deliver it to you). On your own computer (`pnpm dev`) any made-up address works: every email Pactlab sends, invitations and sign-in codes, is written to `apps/api/.data/mail/`.

## Step B1 — Start the Pact as the seller

1. Click **Start a Pact** (top right).
2. Under *Who are you in this deal?* choose **We are selling (or raising)**. Pact name: `Project Riverside Sale` · Base currency: **EUR** → **Next**. (There is no buying-entity step.)
3. **Selling entity** — Legal or trading name: `Riverside Care Partners B.V.` · **Private** · What kind of company is it?: **Healthcare & health tech** → **Next**.
4. **Asking price** — enter the same asking price as Part A, Step 1 (`2200000`) → **Next**.
5. **Review and start** — the Buyer box says *Bid process — you invite buyers once the pact starts* → **Start Pact**.

**You should see:** the **Bidders** page, with no bidders yet.

## Step B2 — Decide what bidders see

On **Bidders**, under **What bidders see**:

| Field | Enter |
|---|---|
| Shared summary | `Riverside Care Partners B.V. operates nine physical-therapy and primary-care practices, paid mostly by government programmes and commercial insurers.` |
| Your data room (link) | `https://dataroom.example/healthcare` (Pactlab is not the data room; this is where you would grant access) |
| NDA | `Mutual NDA (synthetic): everything shared about Riverside Care Partners B.V. stays confidential.` |
| Offer deadline (UTC) | a date a week from today |

→ **Save**.

Then open the **Documents** tab and upload `documents/01-medical-director-agreement.pdf` with **Share with bidders** ticked (it is chosen at upload and cannot be changed later). Upload nothing else as shared — the rest stays with you.

**You should see:** "Saved. Bidders see the shared view once they accept the NDA." On Documents, `01-medical-director-agreement.pdf` is listed.

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
   | Price | `2000000` (EUR 2,000,000) |
   | Currency | `EUR` |
   | Structure (cash, shares, earn-out…) | `Cash at close for 100% of the shares` |
   | Conditions | `Subject to confirmatory diligence and committed financing` |

   → **Submit offer**.
3. **Northline Strategic (synthetic)**: ask `Can you share the last three years of audited accounts?` → **Ask**. Then offer **Price** `1900000` (EUR 1,900,000), **Structure** `80% cash at close, 20% earn-out over 24 months`, **Conditions** `Key-person retention for the founders` → **Submit offer**.
4. **Atlas Growth Equity (synthetic)**: accept the NDA, then type `Outside our sector focus this year.` as the reason → **Pass on this pact**.

**You should see**, as Northline Strategic (synthetic): your own question and offer only — nothing of Harbor Capital Partners (synthetic)'s question or offer, and no sign that Atlas Growth Equity (synthetic) passed. There are no deal tabs; trying `/deals/<id>/bidders` shows nothing of the seller's side.

## Step B5 — Answer the questions

Back as the seller (your normal window), on **Bidders** under **Questions from bidders**:

- Harbor Capital Partners (synthetic)'s question → answer `One customer contract has a change-of-control clause; it is in the shared documents.` → choose **All bidders (without naming who asked)** → **Answer**.
- Northline Strategic (synthetic)'s question → answer `FY2024 and FY2025 are audited; FY2026 closes in December. We will add them to the data room.` → keep **Only Northline Strategic (synthetic)** → **Answer**.

**You should see**, as Northline Strategic (synthetic) (refresh **Your bid**): your private answer, and under *Answered to all bidders* the change-of-control question — without the name of who asked it. Harbor Capital Partners (synthetic) sees the answer to all, but not Northline Strategic (synthetic)'s private one.

## Step B6 — Compare the offers

On **Bidders**, **Offers side by side** sets the two offers next to each other — price, structure, conditions, version. Pactlab does not rank them or recommend one.

**You should see:** Harbor Capital Partners (synthetic) at EUR 2,000,000 and Northline Strategic (synthetic) at EUR 1,900,000; Atlas Growth Equity (synthetic) marked **Passed** with its reason.

## Step B7 — Shortlist, run round 2 and choose

1. Click **Shortlist** on Harbor Capital Partners (synthetic) and on Northline Strategic (synthetic), then **Start round 2 with 2 shortlisted**.
2. As each bidder, submit a revised offer on **Your bid**: Harbor Capital Partners (synthetic) `2100000`, Northline Strategic (synthetic) `1900000` → **Submit revised offer**. Every version stays listed.
3. As the seller, click **Award to Harbor Capital Partners (synthetic)**.

**You should see:** "Awarded. Every other bidder has been declined and their access ended." Harbor Capital Partners (synthetic)'s **Your bid** says **Selected by the seller**; Northline Strategic (synthetic) can no longer open the pact. The **Team** tab and the audit log record every step.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 144 revenue lines, one per payer remittance per month | **Yes** — billing export step |
| `claims-summary.csv` | Monthly claims billed, paid and denial rate by payer (72 rows) | **Yes** — industry data step |
| `provider-roster.csv` | Provider roster, pseudonymous, with credential expiry dates (18 rows) | **Yes** — industry data step |
| `documents/01-medical-director-agreement.pdf` | Medical-director agreement and time records | **Yes** — documents step |
| `documents/02-privacy-risk-assessment.pdf` | Most recent privacy and security risk assessment | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `bidders.csv` | The three bidding firms for Part B: who to invite, what each asks and offers | **No** — read it while you follow Part B |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Notes

- Provider data is pseudonymous and aggregate by design; Pactlab never sends people data to a model.

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
| `02 Finance/Exports/Riverside claims summary export Sep26.csv` | Claims summary |  |
| `02 Finance/Exports/Riverside invoice lines export Sep26.csv` | Invoice lines |  |
| `02 Finance/Mgmt accounts FY26 - Riverside.md` | Income statement (P&L) | Revenue matches the invoice lines for Oct 2025 – Sep 2026. |
| `02 Finance/Riverside FY26 summary.md` | Pactlab asks: income statement or cash flow statement? | Mixes profit and cash flow lines. |
| `03 Commercial/Customers/Medical director agreement (signed copy).pdf` | Duplicate — shown once | Same bytes as the agreement above. |
| `03 Commercial/Customers/Medical director agreement.pdf` | Customer contract |  |
| `05 Policies/Privacy risk assessment.pdf` | Policy |  |

**And on the Intake checklist**, these should show as missing: **Cash flow statement**, **Provider roster**.
Once billing is imported, **Customer contract** shows **Some missing** and names the largest billed customers with no contract in the room.
Click **Ask the seller** (or **Copy request for missing items**) to send the list.
