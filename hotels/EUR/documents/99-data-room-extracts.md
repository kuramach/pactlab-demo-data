Harbourview Hotel Holdings B.V. — data-room extracts (synthetic demo data)

Each page reproduces one structured extract from this folder. All names and figures are fictional.
---page---
operating-history.csv — Monthly operating history from the property-management system

month | rooms_available | rooms_sold | adr | revpar | room_revenue | fb_revenue | gross_operating_profit
2024-10 | 5400 | 3488 | 156.88 | 101.33 | 547191.86 | 103966.45 | 186045.23
2024-11 | 5400 | 2937 | 154.56 | 84.06 | 453942.72 | 86249.12 | 154340.52
2024-12 | 5400 | 2864 | 154.25 | 81.81 | 441774.52 | 83937.16 | 150203.34
2025-01 | 5400 | 2643 | 153.32 | 75.04 | 405234.06 | 76994.47 | 137779.58
2025-02 | 5400 | 2790 | 153.94 | 79.54 | 429497.51 | 81604.53 | 146029.15
2025-03 | 5400 | 3084 | 155.18 | 88.62 | 478569.69 | 90928.24 | 162713.69
2025-04 | 5400 | 3304 | 156.11 | 95.51 | 515772.90 | 97996.85 | 175362.79
2025-05 | 5400 | 3672 | 157.65 | 107.20 | 578895.21 | 109990.09 | 196824.37
2025-06 | 5400 | 4332 | 160.43 | 128.70 | 694996.97 | 132049.42 | 236298.97
2025-07 | 5400 | 4847 | 162.60 | 145.95 | 788108.24 | 149740.57 | 267956.80
2025-08 | 5400 | 4773 | 162.29 | 143.44 | 774600.62 | 147174.12 | 263364.21
2025-09 | 5400 | 3965 | 158.89 | 116.66 | 629989.65 | 119698.03 | 214196.48
2025-10 | 5400 | 3488 | 159.23 | 102.85 | 555399.74 | 105525.95 | 188835.91
2025-11 | 5400 | 2937 | 156.88 | 85.32 | 460751.86 | 87542.85 | 156655.63
2025-12 | 5400 | 2864 | 156.56 | 83.04 | 448401.14 | 85196.22 | 152456.39
2026-01 | 5400 | 2643 | 155.62 | 76.17 | 411312.57 | 78149.39 | 139846.27
2026-02 | 5400 | 2790 | 156.25 | 80.73 | 435939.97 | 82828.59 | 148219.59
2026-03 | 5400 | 3084 | 157.51 | 89.95 | 485748.24 | 92292.17 | 165154.40
2026-04 | 5400 | 3304 | 158.45 | 96.95 | 523509.50 | 99466.81 | 177993.23
2026-05 | 5400 | 3672 | 160.02 | 108.81 | 587578.63 | 111639.94 | 199776.73
2026-06 | 5400 | 4332 | 162.84 | 130.63 | 705421.92 | 134030.16 | 239843.45
2026-07 | 5400 | 4847 | 165.04 | 148.14 | 799929.86 | 151986.67 | 271976.15
2026-08 | 5400 | 4773 | 164.72 | 145.60 | 786219.63 | 149381.73 | 267314.67
2026-09 | 5400 | 3965 | 161.27 | 118.41 | 639439.50 | 121493.51 | 217409.43
---page---
str-benchmark.csv — STR benchmark report against the competitive set, by month

month | occupancy | adr | revpar | comp_set_revpar
2025-10 | 0.646 | 159.23 | 102.85 | 103.88
2025-11 | 0.544 | 156.88 | 85.32 | 86.52
2025-12 | 0.530 | 156.56 | 83.04 | 84.54
2026-01 | 0.490 | 155.62 | 76.17 | 77.86
2026-02 | 0.517 | 156.25 | 80.73 | 82.85
2026-03 | 0.571 | 157.51 | 89.95 | 92.68
2026-04 | 0.612 | 158.45 | 96.95 | 100.29
2026-05 | 0.680 | 160.02 | 108.81 | 113.01
2026-06 | 0.802 | 162.84 | 130.63 | 136.22
2026-07 | 0.898 | 165.04 | 148.14 | 155.09
2026-08 | 0.884 | 164.72 | 145.60 | 153.05
2026-09 | 0.734 | 161.27 | 118.41 | 124.96
---page---
agreements-register.csv — Agreements register: the franchise and management agreements’ term, fees and early-termination penalty

agreement_id | kind | counterparty | effective_on | expires_on | fee_rate | other_fee_rate | termination_fee
MER-2009 | franchise | Meridale Hotels (synthetic) | 2009-12-01 | 2029-12-31 | 0.055 | 0.044 | 2484000.00
CHM-2019 | management | Coastline Hospitality Management (synthetic) | 2019-01-01 | 2034-12-31 | 0.03 | 0.10 | 
---page---
pip-schedule.csv — The brand’s property improvement plan: items, estimated cost and due dates

item_id | area | description | estimated_cost | due_on
PIP-01 | Guestrooms | Replace guestroom soft goods and casegoods to the current brand standard | 1380000.00 | 2027-06-30
PIP-02 | Public areas | Renovate the lobby, bar and meeting rooms | 828000.00 | 2027-09-30
PIP-03 | Exterior | Replace exterior signage and the porte-cochère canopy | 368000.00 | 2028-06-30
PIP-04 | Guestrooms | Refit guest bathrooms with walk-in showers | 736000.00 | 2028-12-31
---page---
capex-budget.csv — The owner’s capital expenditure budget, FY2027 and FY2028, each line naming the PIP item it funds

fiscal_year | line | pip_ref | amount
2027 | Lobby, bar and meeting room renovation | PIP-02 | 828000.00
2027 | Roof membrane replacement |  | 322000.00
2027 | Kitchen equipment |  | 165600.00
2028 | Exterior signage and canopy | PIP-03 | 368000.00
2028 | Lift modernisation |  | 239200.00
---page---
pnl.csv — Profit and loss by calendar year, FY2021 to FY2025

Line | FY2021 | FY2022 | FY2023 | FY2024 | FY2025
Rooms revenue | 6369370.40 | 6464910.96 | 6561884.62 | 6660312.89 | 6760217.59
Food and beverage revenue | 1210180.39 | 1228333.08 | 1246758.08 | 1265459.45 | 1284441.34
Other operating revenue | 318468.52 | 323245.55 | 328094.23 | 333015.64 | 338010.88
Cost of rooms department | 1528648.90 | 1551578.63 | 1574852.31 | 1598475.09 | 1622452.22
Cost of food and beverage | 847126.27 | 859833.16 | 872730.66 | 885821.62 | 899108.94
Franchise and brand fees | 477702.78 | 517192.88 | 564322.08 | 612748.79 | 669261.54
Management fees | 236940.58 | 240494.69 | 244102.11 | 247763.64 | 251480.09
Utilities and energy | 355410.87 | 360742.03 | 366153.16 | 371645.46 | 377220.14
Repairs and maintenance | 315920.77 | 320659.58 | 325469.48 | 330351.52 | 335306.79
General and administrative | 710821.74 | 721484.06 | 732306.32 | 743290.92 | 754440.28
