# Halyard Syndicate Inc. — Startup equity SPV (USD)

**Fictional target.** Halyard Syndicate Inc. is an SPV organizer pooling five investors into Halyard Lumen Seed SPV LLC (synthetic), which takes one line in the seed round of Lumen Labs Inc., a field-service scheduling startup. Offered under Rule 506(c).
Based in Columbus, Ohio, United States; reports in USD. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Before you start

- Download this whole folder (on GitHub: **Code → Download ZIP** at the top of the repository, then unzip).
- Sign in to Pactlab. The steps take about 15 minutes.
- You upload **3 CSV files** and **7 PDFs**. Nothing else.
- **Never upload the `.md` files** in `documents/`. They are the text each PDF is built from; Pactlab reads the PDFs.
- `vdr-index.csv` is for reference only (how a data room would list these files). Do not upload it.
- Text in **bold** below is a button, tab or option exactly as Pactlab shows it.

## Two ways to test this company

- **Part A — Buyer side** (Steps 1 onwards): you are Halyard Syndicate Inc., the sponsor, diligencing the property you are buying and the offering you raise its equity on.
- **Part B — Seller side** ([below](#part-b--seller-side-run-a-bid-process)): you are Lumen Labs Inc., inviting several buyers — they ask questions, then offer or pass, and you choose one. Uses `bidders.csv`.
- Each part starts its own Pact, so you can do either one, or both.

# Part A — Buyer side

## Step 1 — Start the Pact

1. Click **Start a Pact** (top right).
2. **Name the Pact** — Pact name: `Project Halyard` · Base currency: **USD** → **Next**.
3. **Buying entity** — Legal or trading name: `Halyard Syndicate Inc.` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `Lumen Labs Inc.` · **Private** · What kind of company is it?: **Startup equity SPV** → **Next**.
5. **Asking price** — choose **We have an asking price**, then:

   | Field | Enter |
   |---|---|
   | Asking price | `8000000` (USD 8,000,000) |
   | Currency | **USD** |
   | Quoted as | **Enterprise value** |
   | Where it came from | **Teaser or information memorandum** |
   | Date quoted | 30 September 2026 |
   | Of which earn-out, Note | leave empty |

   → **Next**. (This is the round's stated pre-money: the price the vehicle buys in at. The demo shows how far the evidence supports the round.)
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `Lumen Labs Inc.`, with the asking price USD 8,000,000.

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
| 1 | **Upload cap table** | `cap-table.csv` | **Upload and map columns** → **Check every row** | **Import 6 rows** |
| 2 | **Upload monthly financials** | `monthly-financials.csv` | **Upload and map columns** → **Check every row** | **Import 12 rows** |

**You should see** after each import: "… imported … Industry checks ran on them". Some findings may already appear as drafts; that is expected.

## Step 4 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/01-round-summary.pdf` | **business information** | The startup's round summary: size, price, valuation and its headline claims |
| 2 | `documents/02-safe-1.pdf` | **business information** | The signed SAFE from the startup's earlier round |
| 3 | `documents/03-spv-operating-agreement.pdf` | **business information** | The vehicle's operating agreement: fee, carry, expenses and the offering exemption |
| 4 | `documents/04-spv-investor-summary.pdf` | **business information** | The summary of terms given to investors |
| 5 | `documents/05-side-letter-inv-03.pdf` | **business information** | A side letter with one investor |
| 6 | `documents/06-form-d.pdf` | **business information** | The vehicle's Form D filing confirmation |
| 7 | `documents/99-data-room-extracts.pdf` | **financial information** | Every CSV extract in this folder as one paged PDF, so findings can cite a page |

**You should see:** all 7 documents listed on the **Documents** tab.

## Step 5 — Seat the investors and check the vehicle (SPV tab)

Open the **SPV** tab (it appears only on a startup equity SPV).

1. Under **The vehicle**, enter Vehicle name `Halyard Lumen Seed SPV LLC (synthetic)`, and the exits (× post-money) Downside `0.5`, Base `3`, Upside `10` → **Save the vehicle**.
2. Under **Investor seats**, add each seat (one at a time) → **Add seat**:

   | Investor | Reference | Commitment | Accreditation |
   |---|---|---|---|
   | Marlowe Family Office (synthetic) | `INV-01` | `600000` | **Verified by a third party** |
   | Pinecrest Angels LLC (synthetic) | `INV-02` | `500000` | **Verified by a third party** |
   | Quayle Partners (synthetic) | `INV-03` | `450000` | **Verified by a third party** |
   | Rowan Okafor (synthetic) | `INV-04` | `250000` | **Self-certified** |
   | Sable Point Capital (synthetic) | `INV-05` | `150000` | **Verified by a third party** |

3. Click **Run SPV checks**. Drafts appear on **Findings**; a person decides each.
4. **You should see** under **Vehicle economics**: commitments USD 2,000,000 (the seats plus the organizer's USD 50,000), management fee USD 40,000, expenses USD 25,000, invested USD 1,935,000; carry 20% in the agreement against 15% in the summary.
5. Under **Round verification**: the cap table gives 11,400,000 shares after the round against the summary's 11,000,000; SAFE-1 converts into 400,000 shares at its cap.
6. Under **Investor view**, click **Preview** and then **Publish version 1**. The published view holds the round claims, the cap-table check, the vehicle economics and the return scenarios — never the side letter, the seats or any other investor.

## Step 6 — Run the checks and review the findings

1. Open the **Findings** tab → **Run startup equity spv checks**.
2. **You should see exactly these 9 findings** (running the checks again adds nothing):

   1. **Cap table does not add up after the round** — planted defect (a): the round summary states 11,000,000 fully diluted shares after the round; the cap table with SAFE-1 converted gives 11,400,000 — exactly the 400,000 shares SAFE-1 converts into.
   2. **Carried interest in the operating agreement differs from the investor summary** — planted defect (b): 20% in `documents/03-spv-operating-agreement.pdf`, 15% in `documents/04-spv-investor-summary.pdf`.
   3. **Side letter grants preferential terms the summary does not disclose** — planted defect (c): `documents/05-side-letter-inv-03.pdf` waives INV-03's fee; the summary says "Side letters: none." Organizer-side only.
   4. **Accreditation gap in a 506(c) vehicle** — planted defect (d): INV-04 is recorded as self-certified in a Rule 506(c) vehicle (from the seats you enter on the SPV tab).
   5. **Stated pre-money ties to the cap table** — confirmed: USD 1.00 × 8,000,000 pre-round shares is the stated pre-money.
   6. **Prior-round terms match the signed instruments** — confirmed: the summary's SAFE cap and discount match `documents/02-safe-1.pdf`.
   7. **Round claim verified: ARR** — the summary's ARR ties to `invoice-lines.csv` (billed USD 1,512,493 for September 2026).
   8. **Round claim verified: Runway** — 18 months agrees with `monthly-financials.csv`.
   9. **Round claim not verified: Net revenue retention** — a gap: nothing in the evidence checks the 128% claim. Ask the startup for the cohort data.

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 7 — Test the price

1. Open the **Valuation** tab → **New scenario**.
2. Fill in the valuation method's fields — the hint under each field says where its number comes from (usually the **Finances** tab) — and save.
3. Click **Run** on the scenario.

**You should see:** **Asking vs Sextant** — the asking price against the value the evidence supports, before and after the findings you accepted.

# Part B — Seller side: run a bid process

Here you are Lumen Labs Inc. You invite three bidders from `bidders.csv`, share a little, answer their questions and choose one.
Each bidder sees only their own bid — never another bidder's questions, offers or whether they passed. Part B checks that too.

**Addresses.** This folder holds no email addresses. Invite **an address you can read for each firm**: your own address with `+` and the firm's tag from `bidders.csv` added before the @ (for tag `harbor`: *yourname+harbor* at your email domain — Gmail, Outlook and most providers deliver it to you). On your own computer (`pnpm dev`) any made-up address works: every email Pactlab sends, invitations and sign-in codes, is written to `apps/api/.data/mail/`.

## Step B1 — Start the Pact as the seller

1. Click **Start a Pact** (top right).
2. Under *Who are you in this deal?* choose **We are selling (or raising)**. Pact name: `Project Halyard Sale` · Base currency: **USD** → **Next**. (There is no buying-entity step.)
3. **Selling entity** — Legal or trading name: `Lumen Labs Inc.` · **Private** · What kind of company is it?: **Startup equity SPV** → **Next**.
4. **Asking price** — enter the same asking price as Part A, Step 1 (`8000000`) → **Next**.
5. **Review and start** — the Buyer box says *Bid process — you invite buyers once the pact starts* → **Start Pact**.

**You should see:** the **Bidders** page, with no bidders yet.

## Step B2 — Decide what bidders see

On **Bidders**, under **What bidders see**:

| Field | Enter |
|---|---|
| Shared summary | `Halyard Syndicate Inc. is an SPV organizer pooling five investors into Halyard Lumen Seed SPV LLC (synthetic), which takes one line in the seed round of Lumen Labs Inc., a field-service scheduling startup. Offered under Rule 506(c).` |
| Your data room (link) | `https://dataroom.example/startup-spv` (Pactlab is not the data room; this is where you would grant access) |
| NDA | `Mutual NDA (synthetic): everything shared about Lumen Labs Inc. stays confidential.` |
| Offer deadline (UTC) | a date a week from today |

→ **Save**.

Then open the **Documents** tab and upload `documents/01-round-summary.pdf` with **Share with bidders** ticked (it is chosen at upload and cannot be changed later). Upload nothing else as shared — the rest stays with you.

**You should see:** "Saved. Bidders see the shared view once they accept the NDA." On Documents, `01-round-summary.pdf` is listed.

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
   | Price | `7400000` (USD 7,400,000) |
   | Currency | `USD` |
   | Structure (cash, shares, earn-out…) | `Cash at close for 100% of the shares` |
   | Conditions | `Subject to confirmatory diligence and committed financing` |

   → **Submit offer**.
3. **Northline Strategic (synthetic)**: ask `Can you share the last three years of audited accounts?` → **Ask**. Then offer **Price** `6800000` (USD 6,800,000), **Structure** `80% cash at close, 20% earn-out over 24 months`, **Conditions** `Key-person retention for the founders` → **Submit offer**.
4. **Atlas Growth Equity (synthetic)**: accept the NDA, then type `Outside our sector focus this year.` as the reason → **Pass on this pact**.

**You should see**, as Northline Strategic (synthetic): your own question and offer only — nothing of Harbor Capital Partners (synthetic)'s question or offer, and no sign that Atlas Growth Equity (synthetic) passed. There are no deal tabs; trying `/deals/<id>/bidders` shows nothing of the seller's side.

## Step B5 — Answer the questions

Back as the seller (your normal window), on **Bidders** under **Questions from bidders**:

- Harbor Capital Partners (synthetic)'s question → answer `One customer contract has a change-of-control clause; it is in the shared documents.` → choose **All bidders (without naming who asked)** → **Answer**.
- Northline Strategic (synthetic)'s question → answer `FY2024 and FY2025 are audited; FY2026 closes in December. We will add them to the data room.` → keep **Only Northline Strategic (synthetic)** → **Answer**.

**You should see**, as Northline Strategic (synthetic) (refresh **Your bid**): your private answer, and under *Answered to all bidders* the change-of-control question — without the name of who asked it. Harbor Capital Partners (synthetic) sees the answer to all, but not Northline Strategic (synthetic)'s private one.

## Step B6 — Compare the offers

On **Bidders**, **Offers side by side** sets the two offers next to each other — price, structure, conditions, version. Pactlab does not rank them or recommend one.

**You should see:** Harbor Capital Partners (synthetic) at USD 7,400,000 and Northline Strategic (synthetic) at USD 6,800,000; Atlas Growth Equity (synthetic) marked **Passed** with its reason.

## Step B7 — Shortlist, run round 2 and choose

1. Click **Shortlist** on Harbor Capital Partners (synthetic) and on Northline Strategic (synthetic), then **Start round 2 with 2 shortlisted**.
2. As each bidder, submit a revised offer on **Your bid**: Harbor Capital Partners (synthetic) `7800000`, Northline Strategic (synthetic) `7000000` → **Submit revised offer**. Every version stays listed.
3. As the seller, click **Award to Harbor Capital Partners (synthetic)**.

**You should see:** "Awarded. Every other bidder has been declined and their access ended." Harbor Capital Partners (synthetic)'s **Your bid** says **Selected by the seller**; Northline Strategic (synthetic) can no longer open the pact. The **Team** tab and the audit log record every step.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 288 revenue lines, one per customer subscription per month | **Yes** — billing export step |
| `cap-table.csv` | The startup's cap table before the round, one row per security (pseudonymous holders) (6 rows) | **Yes** — industry data step |
| `monthly-financials.csv` | The startup's cash balance and net burn by month (12 rows) | **Yes** — industry data step |
| `documents/01-round-summary.pdf` | The startup's round summary: size, price, valuation and its headline claims | **Yes** — documents step |
| `documents/02-safe-1.pdf` | The signed SAFE from the startup's earlier round | **Yes** — documents step |
| `documents/03-spv-operating-agreement.pdf` | The vehicle's operating agreement: fee, carry, expenses and the offering exemption | **Yes** — documents step |
| `documents/04-spv-investor-summary.pdf` | The summary of terms given to investors | **Yes** — documents step |
| `documents/05-side-letter-inv-03.pdf` | A side letter with one investor | **Yes** — documents step |
| `documents/06-form-d.pdf` | The vehicle's Form D filing confirmation | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `bidders.csv` | The three bidding firms for Part B: who to invite, what each asks and offers | **No** — read it while you follow Part B |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Notes

- Organizer-side pack: you run the vehicle. Investors are seated as guests and see only their own seat and the published investor view; the startup sees the vehicle as one investor and never the investor list.
- Accreditation is tracked, never determined: record what a verification specialist found, with a link and an evidence pointer.
- Return scenarios are computed from the exit paths you state — never a projection or a promise.
- Diligence support only: not legal advice. Pactlab performs no securities-offering, broker-dealer or investment-adviser function.

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
| `01 Corporate/Round summary.pdf` | Round summary or deck |  |
| `01 Corporate/Safe 1.pdf` | SAFE or convertible note |  |
| `02 Finance/Exports/Halyard cap table export Sep26.csv` | Cap table |  |
| `02 Finance/Exports/Halyard invoice lines export Sep26.csv` | Invoice lines |  |
| `02 Finance/Halyard FY26 summary.md` | Pactlab asks: income statement or cash flow statement? | Mixes profit and cash flow lines. |
| `02 Finance/Mgmt accounts FY26 - Halyard.md` | Income statement (P&L) | Revenue matches the invoice lines for Oct 2025 – Sep 2026. |
| `06 Vehicle/Form d.pdf` | Form D filing |  |
| `06 Vehicle/Side letter inv 03.pdf` | Side letter |  |
| `06 Vehicle/Spv investor summary.pdf` | SPV investor summary |  |
| `06 Vehicle/Spv operating agreement.pdf` | SPV operating agreement |  |

**And on the Intake checklist**, these should show as missing: **Cash flow statement**, **Monthly financials**.
Once billing is imported, **Customer contract** shows **Some missing** and names the largest billed customers with no contract in the room.
Click **Ask the seller** (or **Copy request for missing items**) to send the list.
