Calvera Pharmaceuticals Inc. — data-room extracts (synthetic demo data)

Each page reproduces one structured extract from this folder. All names and figures are fictional.
---page---
patent-schedule.csv — Patent families, products and expiry dates

family | product | jurisdiction | type | expiry
PF-01 | Product A | US | composition of matter | 2028-03-31
PF-01 | Product A | EP | composition of matter | 2028-06-30
PF-02 | Product A | US | formulation | 2033-11-30
PF-03 | Product B | US | method of use | 2033-08-31
---page---
pipeline.csv — Development pipeline: each programme's claimed phase and next milestone

programme | indication | phase | next_milestone | expected
PX-410 | Idiopathic pulmonary fibrosis | Phase 2 | Phase 2 interim data | 2027-Q4
PX-210 | Chronic cough | Phase 3 | Top-line data | 2027-Q2
PX-330 | Dry eye | Phase 1 | Phase 2 start | 2027-Q3
---page---
trial-registry.csv — Trial-registry records for the pipeline programmes, as filed

registry_id | programme | phase | status | start_date | primary_completion
CTR-2025-04101 | PX-410 | Phase 1 | recruiting | 2025-03-10 | 2027-02-28
CTR-2023-02103 | PX-210 | Phase 3 | active not recruiting | 2023-11-01 | 2027-05-31
CTR-2024-03301 | PX-330 | Phase 1 | completed | 2024-02-01 | 2026-06-30
---page---
obligations-model.csv — The seller's model of milestones, royalties and licence fees owed

obligation_id | counterparty | kind | trigger | amount | rate | expected
OB-01 | Brennick Biologics (synthetic) | milestone | Phase 3 start (PX-330) | 25000000.00 |  | 2029-Q1
OB-02 | Brennick Biologics (synthetic) | royalty | Net sales of PX-330 |  | 0.06 | 
OB-03 | Brennick Biologics (synthetic) | licence_fee |  | 250000.00 |  | Annually
---page---
rd-roster.csv — R&D roster by pseudonymous reference: programmes led and patent families as inventor

scientist_ref | function | programmes_led | patent_families
S-01 | Discovery chemistry | 2 | 3
S-02 | Clinical development | 1 | 0
S-03 | Formulation | 0 | 1
S-04 | Translational biology | 0 | 0
---page---
pnl.csv — Profit and loss by fiscal year, FY2023 to FY2025

Line | FY2023 | FY2024 | FY2025
Royalty revenue | 5475115.64 | 5920764.58 | 6366413.53
Product supply revenue | 1724715.50 | 1865099.32 | 2005483.14
Licence fee revenue | 433266.78 | 468532.68 | 503798.58
Cost of product supply | 724380.51 | 783341.71 | 822248.09
Research and development | 22000000.00 | 22300000.00 | 22100000.00
Royalties paid to licensors | 160295.06 | 165087.93 | 177513.91
General and administrative | 1450288.60 | 1485791.38 | 1508868.19
