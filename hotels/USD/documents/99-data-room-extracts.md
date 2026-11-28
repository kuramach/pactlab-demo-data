Harbourview Hotel Holdings Inc. — data-room extracts (synthetic demo data)

Each page reproduces one structured extract from this folder. All names and figures are fictional.
---page---
operating-history.csv — Monthly operating history from the property-management system

month | rooms_available | rooms_sold | adr | revpar | room_revenue | fb_revenue | gross_operating_profit
2024-10 | 5400 | 3488 | 170.52 | 110.14 | 594773.76 | 113007.01 | 202223.08
2024-11 | 5400 | 2937 | 168.00 | 91.37 | 493416.00 | 93749.04 | 167761.44
2024-12 | 5400 | 2864 | 167.66 | 88.92 | 480189.70 | 91236.04 | 163264.50
2025-01 | 5400 | 2643 | 166.66 | 81.57 | 440471.81 | 83689.64 | 149760.42
2025-02 | 5400 | 2790 | 167.33 | 86.45 | 466845.12 | 88700.57 | 158727.34
2025-03 | 5400 | 3084 | 168.67 | 96.33 | 520184.45 | 98835.05 | 176862.71
2025-04 | 5400 | 3304 | 169.68 | 103.82 | 560622.72 | 106518.32 | 190611.72
2025-05 | 5400 | 3672 | 171.36 | 116.52 | 629233.92 | 119554.44 | 213939.53
2025-06 | 5400 | 4332 | 174.38 | 139.89 | 755431.49 | 143531.98 | 256846.71
2025-07 | 5400 | 4847 | 176.74 | 158.64 | 856639.39 | 162761.48 | 291257.39
2025-08 | 5400 | 4773 | 176.40 | 155.92 | 841957.20 | 159971.87 | 286265.45
2025-09 | 5400 | 3965 | 172.70 | 126.81 | 684771.36 | 130106.56 | 232822.26
2025-10 | 5400 | 3488 | 173.08 | 111.80 | 603695.37 | 114702.12 | 205256.43
2025-11 | 5400 | 2937 | 170.52 | 92.74 | 500817.24 | 95155.28 | 170277.86
2025-12 | 5400 | 2864 | 170.18 | 90.26 | 487392.54 | 92604.58 | 165713.46
2026-01 | 5400 | 2643 | 169.16 | 82.79 | 447078.89 | 84944.99 | 152006.82
2026-02 | 5400 | 2790 | 169.84 | 87.75 | 473847.80 | 90031.08 | 161108.25
2026-03 | 5400 | 3084 | 171.20 | 97.78 | 527987.21 | 100317.57 | 179515.65
2026-04 | 5400 | 3304 | 172.23 | 105.38 | 569032.06 | 108116.09 | 193470.90
2026-05 | 5400 | 3672 | 173.93 | 118.27 | 638672.43 | 121347.76 | 217148.63
2026-06 | 5400 | 4332 | 177.00 | 141.99 | 766762.96 | 145684.96 | 260699.41
2026-07 | 5400 | 4847 | 179.39 | 161.02 | 869488.98 | 165202.91 | 295626.25
2026-08 | 5400 | 4773 | 179.05 | 158.26 | 854586.56 | 162371.45 | 290559.43
2026-09 | 5400 | 3965 | 175.29 | 128.71 | 695042.93 | 132058.16 | 236314.60
---page---
str-benchmark.csv — STR benchmark report against the competitive set, by month

month | occupancy | adr | revpar | comp_set_revpar
2025-10 | 0.646 | 173.08 | 111.80 | 112.92
2025-11 | 0.544 | 170.52 | 92.74 | 94.04
2025-12 | 0.530 | 170.18 | 90.26 | 91.89
2026-01 | 0.490 | 169.16 | 82.79 | 84.63
2026-02 | 0.517 | 169.84 | 87.75 | 90.05
2026-03 | 0.571 | 171.20 | 97.78 | 100.75
2026-04 | 0.612 | 172.23 | 105.38 | 109.01
2026-05 | 0.680 | 173.93 | 118.27 | 122.84
2026-06 | 0.802 | 177.00 | 141.99 | 148.06
2026-07 | 0.898 | 179.39 | 161.02 | 168.58
2026-08 | 0.884 | 179.05 | 158.26 | 166.35
2026-09 | 0.734 | 175.29 | 128.71 | 135.83
---page---
agreements-register.csv — Agreements register: the franchise and management agreements’ term, fees and early-termination penalty

agreement_id | kind | counterparty | effective_on | expires_on | fee_rate | other_fee_rate | termination_fee
MER-2009 | franchise | Meridale Hotels (synthetic) | 2009-12-01 | 2029-12-31 | 0.055 | 0.044 | 2700000.00
CHM-2019 | management | Coastline Hospitality Management (synthetic) | 2019-01-01 | 2034-12-31 | 0.03 | 0.10 | 
---page---
pip-schedule.csv — The brand’s property improvement plan: items, estimated cost and due dates

item_id | area | description | estimated_cost | due_on
PIP-01 | Guestrooms | Replace guestroom soft goods and casegoods to the current brand standard | 1500000.00 | 2027-06-30
PIP-02 | Public areas | Renovate the lobby, bar and meeting rooms | 900000.00 | 2027-09-30
PIP-03 | Exterior | Replace exterior signage and the porte-cochère canopy | 400000.00 | 2028-06-30
PIP-04 | Guestrooms | Refit guest bathrooms with walk-in showers | 800000.00 | 2028-12-31
---page---
capex-budget.csv — The owner’s capital expenditure budget, FY2027 and FY2028, each line naming the PIP item it funds

fiscal_year | line | pip_ref | amount
2027 | Lobby, bar and meeting room renovation | PIP-02 | 900000.00
2027 | Roof membrane replacement |  | 350000.00
2027 | Kitchen equipment |  | 180000.00
2028 | Exterior signage and canopy | PIP-03 | 400000.00
2028 | Lift modernisation |  | 260000.00
---page---
pnl.csv — Profit and loss by calendar year, FY2021 to FY2025

Line | FY2021 | FY2022 | FY2023 | FY2024 | FY2025
Rooms revenue | 6923228.73 | 7027077.15 | 7132483.32 | 7239470.56 | 7348062.61
Food and beverage revenue | 1315413.45 | 1335144.66 | 1355171.85 | 1375499.40 | 1396131.89
Other operating revenue | 346161.44 | 351353.86 | 356624.17 | 361973.53 | 367403.13
Cost of rooms department | 1661574.90 | 1686498.52 | 1711796.00 | 1737472.93 | 1763535.03
Cost of food and beverage | 920789.42 | 934601.26 | 948620.30 | 962849.58 | 977292.32
Franchise and brand fees | 519242.15 | 562166.17 | 613393.57 | 666031.29 | 727458.20
Management fees | 257544.11 | 261407.27 | 265328.38 | 269308.30 | 273347.93
Utilities and energy | 386316.16 | 392110.91 | 397992.57 | 403962.46 | 410021.89
Repairs and maintenance | 343392.14 | 348543.03 | 353771.17 | 359077.74 | 364463.91
General and administrative | 772632.33 | 784221.81 | 795985.14 | 807924.91 | 820043.79
