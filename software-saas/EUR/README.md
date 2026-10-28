# Brightwave Software B.V. — Software and SaaS (EUR)

**Fictional target.** Brightwave Software B.V. sells workflow software to mid-sized logistics and services firms on monthly and annual subscriptions.
Based in Utrecht, the Netherlands; reports in EUR. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Before you start

- Download this whole folder (on GitHub: **Code → Download ZIP** at the top of the repository, then unzip).
- Sign in to Pactlab. The steps take about 15 minutes.
- You upload **1 CSV file** and **3 PDFs**. Nothing else.
- **Never upload the `.md` files** in `documents/`. They are the text each PDF is built from; Pactlab reads the PDFs.
- `vdr-index.csv` is for reference only (how a data room would list these files). Do not upload it.
- Text in **bold** below is a button, tab or option exactly as Pactlab shows it.

## Two ways to test this company

- **Part A — Buyer side** (Steps 1 onwards): you are a buyer doing diligence on Brightwave Software B.V..
- **Part B — Seller side** ([below](#part-b--seller-side-run-a-bid-process)): you are Brightwave Software B.V., inviting several buyers — they ask questions, then offer or pass, and you choose one. Uses `bidders.csv`.
- Each part starts its own Pact, so you can do either one, or both.

# Part A — Buyer side

## Step 1 — Start the Pact

1. Click **Start a Pact** (top right).
2. **Name the Pact** — Pact name: `Project Brightwave` · Base currency: **EUR** → **Next**.
3. **Buying entity** — Legal or trading name: `Demo Buyer` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `Brightwave Software B.V.` · **Private** · What kind of company is it?: **Software & SaaS** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `4600000` (EUR 4,600,000) |
   | Currency | **EUR** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the seller's ask: 8× the September 2026 billed revenue run-rate. The demo shows how far the evidence supports it.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `Brightwave Software B.V.`, with the asking price EUR 4,600,000.

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

   1. **Management ARR exceeds billed ARR** — the KPI pack reports EUR 603,623; `invoice-lines.csv` supports EUR 579,887 at September 2026 — a gap of EUR 23,736. The KPI pack still counts Quarry Lane Studios, whose last invoice was June 2026.
   2. **Revenue concentration** — Harborline Freight (synthetic) is 27.6% of September 2026 billed revenue.
   3. **Largest customer can leave on a sale** — `documents/02-master-services-agreement-northgate.pdf` page 2, clause 14 — termination on change of control.
   4. **Contraction hidden in the logo count** — Amberline Hotels drops by 30% from April 2026; the KPI pack reports 14 active customers, the ledger has 13.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 6 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

# Part B — Seller side: run a bid process

Here you are Brightwave Software B.V. You invite three bidders from `bidders.csv`, share a little, answer their questions and choose one.
Each bidder sees only their own bid — never another bidder's questions, offers or whether they passed. Part B checks that too.

**Addresses.** This folder holds no email addresses. Invite **an address you can read for each firm**: your own address with `+` and the firm's tag from `bidders.csv` added before the @ (for tag `harbor`: *yourname+harbor* at your email domain — Gmail, Outlook and most providers deliver it to you). On your own computer (`pnpm dev`) any made-up address works: every email Pactlab sends, invitations and sign-in codes, is written to `apps/api/.data/mail/`.

## Step B1 — Start the Pact as the seller

1. Click **Start a Pact** (top right).
2. Under *Who are you in this deal?* choose **We are selling (or raising)**. Pact name: `Project Brightwave Sale` · Base currency: **EUR** → **Next**. (There is no buying-entity step.)
3. **Selling entity** — Legal or trading name: `Brightwave Software B.V.` · **Private** · What kind of company is it?: **Software & SaaS** → **Next**.
4. **Asking price** — enter the same asking price as Part A, Step 1 (`4600000`) → **Next**.
5. **Review and start** — the Buyer box says *Bid process — you invite buyers once the pact starts* → **Start Pact**.

**You should see:** the **Bidders** page, with no bidders yet.

## Step B2 — Decide what bidders see

On **Bidders**, under **What bidders see**:

| Field | Enter |
|---|---|
| Shared summary | `Brightwave Software B.V. sells workflow software to mid-sized logistics and services firms on monthly and annual subscriptions.` |
| Your data room (link) | `https://dataroom.example/software-saas` (Pactlab is not the data room; this is where you would grant access) |
| NDA | `Mutual NDA (synthetic): everything shared about Brightwave Software B.V. stays confidential.` |
| Offer deadline (UTC) | a date a week from today |

→ **Save**.

Then open the **Documents** tab and upload `documents/01-board-kpi-pack-2026-09.pdf` with **Share with bidders** ticked (it is chosen at upload and cannot be changed later). Upload nothing else as shared — the rest stays with you.

**You should see:** "Saved. Bidders see the shared view once they accept the NDA." On Documents, `01-board-kpi-pack-2026-09.pdf` is listed.

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
   | Price | `4200000` (EUR 4,200,000) |
   | Currency | `EUR` |
   | Structure (cash, shares, earn-out…) | `Cash at close for 100% of the shares` |
   | Conditions | `Subject to confirmatory diligence and committed financing` |

   → **Submit offer**.
3. **Northline Strategic (synthetic)**: ask `Can you share the last three years of audited accounts?` → **Ask**. Then offer **Price** `3900000` (EUR 3,900,000), **Structure** `80% cash at close, 20% earn-out over 24 months`, **Conditions** `Key-person retention for the founders` → **Submit offer**.
4. **Atlas Growth Equity (synthetic)**: accept the NDA, then type `Outside our sector focus this year.` as the reason → **Pass on this pact**.

**You should see**, as Northline Strategic (synthetic): your own question and offer only — nothing of Harbor Capital Partners (synthetic)'s question or offer, and no sign that Atlas Growth Equity (synthetic) passed. There are no deal tabs; trying `/deals/<id>/bidders` shows nothing of the seller's side.

## Step B5 — Answer the questions

Back as the seller (your normal window), on **Bidders** under **Questions from bidders**:

- Harbor Capital Partners (synthetic)'s question → answer `One customer contract has a change-of-control clause; it is in the shared documents.` → choose **All bidders (without naming who asked)** → **Answer**.
- Northline Strategic (synthetic)'s question → answer `FY2024 and FY2025 are audited; FY2026 closes in December. We will add them to the data room.` → keep **Only Northline Strategic (synthetic)** → **Answer**.

**You should see**, as Northline Strategic (synthetic) (refresh **Your bid**): your private answer, and under *Answered to all bidders* the change-of-control question — without the name of who asked it. Harbor Capital Partners (synthetic) sees the answer to all, but not Northline Strategic (synthetic)'s private one.

## Step B6 — Compare the offers

On **Bidders**, **Offers side by side** sets the two offers next to each other — price, structure, conditions, version. Pactlab does not rank them or recommend one.

**You should see:** Harbor Capital Partners (synthetic) at EUR 4,200,000 and Northline Strategic (synthetic) at EUR 3,900,000; Atlas Growth Equity (synthetic) marked **Passed** with its reason.

## Step B7 — Shortlist, run round 2 and choose

1. Click **Shortlist** on Harbor Capital Partners (synthetic) and on Northline Strategic (synthetic), then **Start round 2 with 2 shortlisted**.
2. As each bidder, submit a revised offer on **Your bid**: Harbor Capital Partners (synthetic) `4500000`, Northline Strategic (synthetic) `4000000` → **Submit revised offer**. Every version stays listed.
3. As the seller, click **Award to Harbor Capital Partners (synthetic)**.

**You should see:** "Awarded. Every other bidder has been declined and their access ended." Harbor Capital Partners (synthetic)'s **Your bid** says **Selected by the seller**; Northline Strategic (synthetic) can no longer open the pact. The **Team** tab and the audit log record every step.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 302 revenue lines, one per customer subscription per month | **Yes** — billing export step |
| `documents/01-board-kpi-pack-2026-09.pdf` | Management KPI pack with reported ARR | **Yes** — documents step |
| `documents/02-master-services-agreement-northgate.pdf` | Largest customer contract, with change-of-control clause | **Yes** — documents step |
| `documents/03-balance-sheet-2026-09-30.pdf` | Balance sheet with debt and debt-like items | **Yes** — documents step |
| `bidders.csv` | The three bidding firms for Part B: who to invite, what each asks and offers | **No** — read it while you follow Part B |
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
