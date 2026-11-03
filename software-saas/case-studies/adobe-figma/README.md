# Case study: Adobe and Figma (2022–2023), a SaaS pact that did not close

> **Public record, not synthetic data.** Unlike the rest of this repository, this case study names real companies. Every fact comes from a public source listed in [`sources.csv`](sources.csv) and is cited next to it. There are no internal documents, invented figures or data-room files here. Lines marked **Pactlab calculation** are simple arithmetic on cited figures. The section *What Pactlab learns* is Pactlab's own analysis. Pactlab is not affiliated with Adobe or Figma.

Pactlab case studies record what we learn from good and bad pact outcomes, and how Pactlab can protect future pacts.

## At a glance

| | |
|---|---|
| Buyer | Adobe Inc. |
| Target | Figma, Inc., a browser-first collaborative design platform |
| Signed | 15 September 2022 [S1] |
| Price | About USD 20 billion, roughly half cash and half stock [S1] |
| Figma at signing (as stated by Adobe) | ARR expected above USD 400 million exiting 2022; net dollar retention above 150%; gross margin about 90% [S1] |
| Price over ARR | About 50× (Pactlab calculation from [S1]) |
| Outcome | Terminated by mutual agreement on 17 December 2023 [S2] |
| Why | "No clear path to receive necessary regulatory approvals from the European Commission and the UK Competition and Markets Authority" [S3] |
| Cost to the buyer | USD 1 billion termination fee paid to Figma [S2], about 5% of the price (Pactlab calculation) |
| Signing to termination | About 15 months |

## What happened

1. **The deal (September 2022).** Adobe agreed to buy Figma for about USD 20 billion, roughly half cash and half stock. It expected to close in 2023, subject to regulatory approvals [S1].
   - **Retention:** about 6 million additional Adobe restricted stock units for Figma's CEO and employees, vesting over four years *after closing* [S1].
   - **Leadership:** Dylan Field was to keep leading Figma [S1].
2. **The UK review (May–November 2023).**
   - **Phase 1:** the CMA opened a merger inquiry on 3 May 2023. On 30 June it found the deal may be expected to substantially lessen competition [S4].
   - **Phase 2:** the CMA referred the deal to an in-depth investigation on 13 July [S4].
   - **Provisional findings, 28 November [S4, S5]:**
     - the deal would eliminate competition between two key competitors in product design, image editing and illustration software;
     - remedies could include blocking the deal.
3. **The EU review (August–November 2023).** The European Commission opened an in-depth investigation on 7 August 2023 into the market for interactive product design software [S6, S7]. It sent Adobe a Statement of Objections on 17 November [S6].
4. **Termination (December 2023).** On 17 December the companies agreed to terminate the merger agreement. Adobe paid the agreed USD 1 billion termination fee within three business days [S2]. In the joint announcement, Adobe's CEO said the companies "strongly disagree with the recent regulatory findings" but would "move forward independently" [S3]. The Commission closed its investigation on 18 December [S7], and the CMA published the cancellation of its reference on 19 December [S4].
5. **Afterwards.**
   - **Figma's results:** revenue of USD 504.9 million in 2023 and USD 749 million in 2024 (48% growth), and net dollar retention of 132% at 31 March 2025 [S8, S9].
   - **IPO:** Figma listed on the NYSE on 31 July 2025 at USD 33 a share, and closed its first day at USD 115.50 [S10].

The dated events are in [`timeline.csv`](timeline.csv), the terms in [`deal-terms.csv`](deal-terms.csv) and the disclosed metrics in [`figma-metrics.csv`](figma-metrics.csv). Every row names its sources.

## What Pactlab learns

Pactlab's loop runs: **evidence → finding → assumption → valuation scenario → deal term → integration action.** Here is how each lesson from this pact maps onto it.

1. **Product overlap is a regulatory finding from day one, not a closing formality.**
   - **What happened:** both regulators centred on the two companies competing in the same design software [S5, S6].
   - **For Pactlab:** a buyer that already sells a product in the target's market should start with a cited **REGULATORY** finding, before any regulator does.
   - **How to test it:** an explicit assumption (the chance of clearance, and how long it takes), and a scenario in which the deal does not close.
2. **Price the walk-away, not just the deal.**
   - **What happened:** the termination fee was USD 1 billion, about 5% of the price [S1, S2]. It was money the buyer paid for a deal it did not get.
   - **For Pactlab:** a reverse termination fee is a priced risk for the buyer and a protection for the seller. Size it against the clearance assumption, side by side with the outside date and any remedy commitments.
3. **Time is a cost.**
   - **What happened:** about 15 months passed between signing and termination.
   - **Why it matters:** the retention equity vested only after closing [S1], so for 15 months it held no one.
   - **For Pactlab:** pacts with a long regulatory path need an integration action that does not depend on closing. Examples: a retention plan for the waiting period, and a decision on what each side may build in the meantime.
4. **Date every seller statement, and check it against later evidence.**
   - **What happened:** at signing, Adobe stated Figma's net dollar retention as above 150% (2022) [S1]. Figma's own S-1 later reported 132% at 31 March 2025 [S8, S9]. These are different periods, and both may be accurate.
   - **For Pactlab:** this is why it records seller statements as dated claims, checked against the evidence, rather than as facts.
5. **A failed pact can still create value — for the other side.**
   - **What happened:** the target received the termination fee and later went public [S2, S10].
   - **For Pactlab:** when Pactlab compares the asking price with the value the evidence supports, the cost of not closing belongs in the buyer's scenarios.

## Replay it in Pactlab

There's no data room for this pact: the companies' internal records are not public, and we do not invent them for real companies. To practise these lessons:

1. Use the synthetic Software & SaaS demo ([USD](../../USD/), [EUR](../../EUR/), [GBP](../../GBP/)).
2. Add what this case study teaches:
   - a regulatory finding for an overlapping product;
   - an assumption for the chance of clearance;
   - a scenario in which the deal fails and the buyer pays a termination fee;
   - proposed terms for the fee and the outside date.

## Files

| File | What it is |
|---|---|
| `timeline.csv` | Dated events, each with its sources |
| `deal-terms.csv` | Announced and termination terms; calculations marked as such |
| `figma-metrics.csv` | Metrics disclosed publicly, with the date each refers to |
| `sources.csv` | Every source: publisher, date, primary or secondary, URL and licence |

## Licence and attribution

- **What is CC0:** the text and the compiled tables in this folder, like the rest of the repository. Facts themselves are not owned.
- **Third-party documents:** none are reproduced here. Each source is linked and keeps its own terms.
- **CMA material:** used under the [Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/), © Crown copyright.
- **Quotations:** short ones only, from the cited filings and press releases.
- **Trademarks:** Adobe and Figma are trademarks of their owners.
- **Corrections:** if a fact here is wrong or out of date, open an issue with the source.
