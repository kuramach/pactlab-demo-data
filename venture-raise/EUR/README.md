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
| `documents/*.md` | The text each PDF is built from | **No** — never |
| `vdr-index.csv` | Index of every file, as a data room would list it | **No** — reference only |

## Notes

- Founder-side pack: the founder is the Pactlab user and investors are the counterparty. Drags are what an investor will find; cushions stay confidential until the founder shares them.
- Holders in the cap table are pseudonymous references (F-1, E-02, I-3); no names.
