# Loopwise B.V. — Venture Raise (EUR)

**Fictional target.** Loopwise B.V. is a seed-stage SaaS startup: scheduling and invoicing for field-service teams, raising a seed round from angels, an accelerator and venture funds.
Based in Utrecht, the Netherlands; reports in EUR. Data runs October 2024 to September 2026.

> Synthetic demo data. Every company, person, address, account and figure here is invented.

## Before you start

- Download this whole folder (on GitHub: **Code → Download ZIP** at the top of the repository, then unzip).
- Sign in to Pactlab. The steps take about 15 minutes.
- You upload **3 CSV files** and **8 PDFs**. Nothing else.
- **Never upload the `.md` files** in `documents/`. They are the text each PDF is built from; Pactlab reads the PDFs.
- `vdr-index.csv` is for reference only (how a data room would list these files). Do not upload it.
- Text in **bold** below is a button, tab or option exactly as Pactlab shows it.

## Two ways to test this company

- **Part A — Buyer side** (Steps 1 onwards): you are the founder, diligencing your own startup before investors do.
- **Part B — Seller side** ([below](#part-b--seller-side-run-a-round)): you are the founder, inviting several investors — they ask questions, then offer or pass, and you choose one. Uses `bidders.csv`.
- Each part starts its own Pact, so you can do either one, or both.

# Part A — Buyer side

## Step 1 — Start the Pact

1. Click **Start a Pact** (top right).
2. **Name the Pact** — Pact name: `Project Loopwise` · Base currency: **EUR** → **Next**.
3. **Buying entity** — Legal or trading name: `Demo Buyer` · **Private** → **Next**.
4. **Selling entity** — Legal or trading name: `Loopwise B.V.` · **Private** · What kind of company is it?: **Venture Raise** → **Next**.
5. **Asking price** — choose **Not known yet** (a raise has no asking price; you set your round on the **Raise** tab after the uploads) → **Next**.
6. **Review and start** — check the summary → **Start Pact**.

**You should see:** the Pact overview for `Loopwise B.V.`.

## Step 2 — Upload the billing export

1. Open the **Sources** tab → **Upload billing export**.
2. *1. Where is the export from?* → **Pactlab standard template**.
3. *2. Choose the file* → `invoice-lines.csv` → **Upload and map columns**.
4. The columns are matched for you. Click **Check every row**, then **Import 336 lines**.

**You should see:** a green message ending "Finances now include them." The **Finances** tab now shows the revenue ledger.

## Step 3 — Upload the industry data

Open the **Sources** tab and scroll to **Industry data**. Upload these files one at a time:

| # | Click | Choose the file | Then | Button should read |
|---|---|---|---|---|
| 1 | **Upload cap table** | `cap-table.csv` | **Upload and map columns** → **Check every row** | **Import 9 rows** |
| 2 | **Upload monthly financials** | `monthly-financials.csv` | **Upload and map columns** → **Check every row** | **Import 12 rows** |

**You should see** after each import: "… imported … Industry checks ran on them". Some findings may already appear as drafts; that is expected.

## Step 4 — Upload the documents

Open the **Documents** tab. Under **Upload a document**, upload each PDF from the `documents/` folder, one at a time — choose the file, set **Data class**, leave **Keep away from AI** unticked, click **Upload**.

| # | File | Data class | What it is |
|---|---|---|---|
| 1 | `documents/01-investor-deck.pdf` | **business information** | Seed round investor deck with headline metrics |
| 2 | `documents/02-certificate-of-incorporation.pdf` | **business information** | Certificate of incorporation with issued shares |
| 3 | `documents/03-contractor-agreement-northbeam.pdf` | **business information** | Contractor agreement with IP assignment |
| 4 | `documents/04-contractor-agreement-quillfield.pdf` | **business information** | Contractor agreement for app design |
| 5 | `documents/05-83b-confirmations.pdf` | **business information** | Founders 83(b) election confirmations |
| 6 | `documents/06-term-sheet-harborline.pdf` | **business information** | Seed term sheet received from a venture fund |
| 7 | `documents/07-safe-register.pdf` | **business information** | Register of SAFEs signed before this round |
| 8 | `documents/99-data-room-extracts.pdf` | **financial information** | Every CSV extract in this folder as one paged PDF, so findings can cite a page |

**You should see:** all 8 documents listed on the **Documents** tab.

## Step 5 — Set your round and record the offer (Raise tab)

Open the **Raise** tab.

1. Under **The round**, enter:

   | Field | Enter |
   |---|---|
   | Currency | **EUR** |
   | Your ask (pre-money) | `11040000` (EUR 11,040,000) |
   | Raising | `1840000` (EUR 1,840,000) |
   | Pool target after the round (%) | `10` |

   → **Save round**.
2. Under **Offers**, record Harborline Ventures' term sheet (`documents/06-term-sheet-harborline.pdf`):

   | Field | Enter |
   |---|---|
   | Investor (firm or fund) | `Harborline Ventures` |
   | Pre-money (EUR) | `9200000` (EUR 9,200,000) |
   | Amount (EUR) | `1840000` (EUR 1,840,000) |
   | Pool target (%) | `10` |
   | Liquidation preference (×) | `1` |
   | Investor board seats | `1` |
   | Received on | 30 September 2026 |

   → **Record offer**.

**You should see:** **Offers side by side** showing Harborline's price per share and what the founders own after the round.

## Step 6 — Run the checks and review the findings

1. Open the **Findings** tab → **Run venture raise checks**.
2. **You should see exactly these 6 findings** (running the checks again adds nothing):

   1. **Deck ARR contradicted by billing** — the deck states EUR 1,520,000; `invoice-lines.csv` bills EUR 1,447,565 ARR for September 2026 (`documents/01-investor-deck.pdf` page 2).
   2. **SAFE stack converts into more than expected** — SAFE-1 has a most-favoured-nation clause, so it takes SAFE-3's lower cap (`cap-table.csv`, `documents/07-safe-register.pdf`).
   3. **IP assignment gap** — the Quillfield Design agreement has no IP assignment (`documents/04-contractor-agreement-quillfield.pdf`).
   4. **Runway shorter than the deck says** — the deck states 18 months; `monthly-financials.csv` gives 12.3 months at the last three months' burn.
   5. **Cap table reconciles to the corporate record** — confirmed value (+1, founder-confidential): 9,000,000 issued shares in `cap-table.csv` match `documents/02-certificate-of-incorporation.pdf`.
   6. **Board composition after the round** — informational: two founder directors and one investor director (`documents/06-term-sheet-harborline.pdf` page 2).

3. Open each finding, read the quoted evidence, then click **Accept**, **Reject** or **Ask for support**. A person decides; Pactlab only drafts.

## Step 7 — Test the price

Open the **Raise** tab again. **Offers side by side** now reflects the cap table: SAFE-1 converts on SAFE-3's terms (most-favoured-nation). Under **Ready for diligence?**, see what an investor will still ask for. The investor view shares only what is safe to share.

# Part B — Seller side: run a round

Here you are Loopwise B.V raising a round. You invite three investors from `bidders.csv`, share a little, answer their questions and choose one.
Each investor sees only their own bid — never another investor's questions, offers or whether they passed. Part B checks that too.

**Addresses.** This folder holds no email addresses. Invite **an address you can read for each firm**: your own address with `+` and the firm's tag from `bidders.csv` added before the @ (for tag `harbor`: *yourname+harbor* at your email domain — Gmail, Outlook and most providers deliver it to you). On your own computer (`pnpm dev`) any made-up address works: every email Pactlab sends, invitations and sign-in codes, is written to `apps/api/.data/mail/`.

## Step B1 — Start the Pact as the seller

1. Click **Start a Pact** (top right).
2. Under *Who are you in this deal?* choose **We are selling (or raising)**. Pact name: `Project Loopwise Sale` · Base currency: **EUR** → **Next**. (There is no buying-entity step.)
3. **Selling entity** — Legal or trading name: `Loopwise B.V.` · **Private** · What kind of company is it?: **Venture Raise** → **Next**.
4. **Asking price** — choose **Not known yet** → **Next**.
5. **Review and start** — the Buyer box says *Bid process — you invite buyers once the pact starts* → **Start Pact**.

**You should see:** the **Bidders** page, with no bidders yet.

## Step B2 — Decide what investors see

On **Bidders**, under **What bidders see**:

| Field | Enter |
|---|---|
| Shared summary | `Loopwise B.V. is a seed-stage SaaS startup: scheduling and invoicing for field-service teams, raising a seed round from angels, an accelerator and venture funds.` |
| Your data room (link) | `https://dataroom.example/venture-raise` (Pactlab is not the data room; this is where you would grant access) |
| NDA | `Mutual NDA (synthetic): everything shared about Loopwise B.V. stays confidential.` |
| Offer deadline (UTC) | a date a week from today |

→ **Save**.

Then open the **Documents** tab and upload `documents/01-investor-deck.pdf` with **Share with bidders** ticked (it is chosen at upload and cannot be changed later). Upload nothing else as shared — the rest stays with you.

**You should see:** "Saved. Bidders see the shared view once they accept the NDA." On Documents, `01-investor-deck.pdf` is listed.

## Step B3 — Add the three investors and invite them

On **Bidders**, for each row of `bidders.csv`:

| Bidding firm | Then invite | Tag |
|---|---|---|
| `Harborline Ventures (synthetic)` → **Add bidder** | your address with `+harborline` in *Invite someone from Harborline Ventures (synthetic)* → **Invite** | `harborline` |
| `Kestrel Seed Fund (synthetic)` → **Add bidder** | your address with `+kestrel` in *Invite someone from Kestrel Seed Fund (synthetic)* → **Invite** | `kestrel` |
| `Atlas Angels (synthetic)` → **Add bidder** | your address with `+atlas` in *Invite someone from Atlas Angels (synthetic)* → **Invite** | `atlas` |

**You should see:** three firms marked **Invited**, each listing the address you invited.

## Step B4 — Be each investor (a private window per investor)

For each investor: open the invitation link (from the email, or the newest file in `apps/api/.data/mail/`) in a **private window**, create the account with the firm's name, sign in with the code, then **Accept and open the pact**.

1. You land on **Your bid** and see only the NDA. Click **I accept the NDA** — the shared summary, the data-room link and the shared document appear.
2. **Harborline Ventures (synthetic)**: ask `How many months of runway do you have after this round?` → **Ask**. Then offer:

   | Field | Enter |
   |---|---|
   | Price | `1840000` (EUR 1,840,000) — the amount invested |
   | Currency | `EUR` |
   | Pre-money valuation (investment rounds only) | `9200000` (EUR 9,200,000) |
   | Structure (cash, shares, earn-out…) | `Series Seed preferred, 1x non-participating` |
   | Conditions | `One investor board seat; pro-rata rights` |

   → **Submit offer**.
3. **Kestrel Seed Fund (synthetic)**: ask `Can you share the founders' vesting schedules?` → **Ask**. Then offer **Price** `1380000` (EUR 1,380,000), **Pre-money** `8280000`, **Structure** `SAFE, valuation cap as the pre-money, 15% discount`, **Conditions** `Most-favoured-nation clause` → **Submit offer**.
4. **Atlas Angels (synthetic)**: accept the NDA, then type `Too early for our fund this year.` as the reason → **Pass on this pact**.

**You should see**, as Kestrel Seed Fund (synthetic): your own question and offer only — nothing of Harborline Ventures (synthetic)'s question or offer, and no sign that Atlas Angels (synthetic) passed. There are no deal tabs; trying `/deals/<id>/bidders` shows nothing of the seller's side.

## Step B5 — Answer the questions

Back as the seller (your normal window), on **Bidders** under **Questions from bidders**:

- Harborline Ventures (synthetic)'s question → answer `About 20 months at the current burn, by our own estimate.` → choose **All bidders (without naming who asked)** → **Answer**.
- Kestrel Seed Fund (synthetic)'s question → answer `Four years with a one-year cliff, from February 2023; the schedules are in the data room.` → keep **Only Kestrel Seed Fund (synthetic)** → **Answer**.

**You should see**, as Kestrel Seed Fund (synthetic) (refresh **Your bid**): your private answer, and under *Answered to all bidders* the runway question — without the name of who asked it. Harborline Ventures (synthetic) sees the answer to all, but not Kestrel Seed Fund (synthetic)'s private one.

## Step B6 — Compare the offers

On **Bidders**, **Offers side by side** sets the two offers next to each other — price, pre-money, structure, conditions, version. Pactlab does not rank them or recommend one.

**You should see:** Harborline Ventures (synthetic) at EUR 1,840,000 and Kestrel Seed Fund (synthetic) at EUR 1,380,000; Atlas Angels (synthetic) marked **Passed** with its reason.

For each investor, click **Add to round comparison**. Open the **Raise** tab: both appear under **Offers**. To see what the founders own after each, import `cap-table.csv` on **Sources** first, as in Part A.

## Step B7 — Shortlist, run round 2 and choose

1. Click **Shortlist** on Harborline Ventures (synthetic) and on Kestrel Seed Fund (synthetic), then **Start round 2 with 2 shortlisted**.
2. As each investor, submit a revised offer on **Your bid**: Harborline Ventures (synthetic) `1840000` (pre-money `10120000`), Kestrel Seed Fund (synthetic) `1380000` (pre-money `8740000`) → **Submit revised offer**. Every version stays listed.
3. As the seller, click **Award to Harborline Ventures (synthetic)**.

**You should see:** "Awarded. Every other bidder has been declined and their access ended." Harborline Ventures (synthetic)'s **Your bid** says **Selected by the seller**; Kestrel Seed Fund (synthetic) can no longer open the pact. The **Team** tab and the audit log record every step.

## Every file in this folder

| File | What it is | Upload it? |
|---|---|---|
| `invoice-lines.csv` | 336 revenue lines, one per customer subscription per month | **Yes** — billing export step |
| `cap-table.csv` | Cap table, one row per security (pseudonymous holders) (9 rows) | **Yes** — industry data step |
| `monthly-financials.csv` | Cash balance and net burn by month (12 rows) | **Yes** — industry data step |
| `documents/01-investor-deck.pdf` | Seed round investor deck with headline metrics | **Yes** — documents step |
| `documents/02-certificate-of-incorporation.pdf` | Certificate of incorporation with issued shares | **Yes** — documents step |
| `documents/03-contractor-agreement-northbeam.pdf` | Contractor agreement with IP assignment | **Yes** — documents step |
| `documents/04-contractor-agreement-quillfield.pdf` | Contractor agreement for app design | **Yes** — documents step |
| `documents/05-83b-confirmations.pdf` | Founders 83(b) election confirmations | **Yes** — documents step |
| `documents/06-term-sheet-harborline.pdf` | Seed term sheet received from a venture fund | **Yes** — documents step |
| `documents/07-safe-register.pdf` | Register of SAFEs signed before this round | **Yes** — documents step |
| `documents/99-data-room-extracts.pdf` | Every CSV extract in this folder as one paged PDF, so findings can cite a page | **Yes** — documents step |
| `bidders.csv` | The three bidding firms for Part B: who to invite, what each asks and offers | **No** — read it while you follow Part B |
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Notes

- Founder-side pack: the founder is the Pactlab user and investors are the counterparty. Drags are what an investor will find; cushions stay confidential until the founder shares them.
- Holders in the cap table are pseudonymous references (F-1, E-02, I-3); no names.

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
| `01 Corporate/83b confirmations.pdf` | Corporate record |  |
| `01 Corporate/Certificate of incorporation.pdf` | Corporate record |  |
| `01 Corporate/Safe register.pdf` | Corporate record |  |
| `01 Corporate/Term sheet harborline.pdf` | Corporate record |  |
| `02 Finance/Exports/Loopwise cap table export Sep26.csv` | Cap table |  |
| `02 Finance/Exports/Loopwise invoice lines export Sep26.csv` | Invoice lines |  |
| `02 Finance/Investor deck.pdf` | Other |  |
| `02 Finance/Loopwise FY26 summary.md` | Pactlab asks: income statement or cash flow statement? | Mixes profit and cash flow lines. |
| `02 Finance/Mgmt accounts FY26 - Loopwise.md` | Income statement (P&L) | Revenue matches the invoice lines for Oct 2025 – Sep 2026. |
| `03 Commercial/Suppliers/Contractor agreement northbeam.pdf` | Supplier contract |  |
| `03 Commercial/Suppliers/Contractor agreement quillfield.pdf` | Supplier contract |  |

**And on the Intake checklist**, these should show as missing: **Cash flow statement**, **Monthly financials**.
Once billing is imported, **Customer contract** shows **Some missing** and names the largest billed customers with no contract in the room.
Click **Ask the seller** (or **Copy request for missing items**) to send the list.
