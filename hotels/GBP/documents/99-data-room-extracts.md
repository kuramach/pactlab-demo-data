Harbourview Hotel Holdings Ltd — data-room extracts (synthetic demo data)

Each page reproduces one structured extract from this folder. All names and figures are fictional.
---page---
operating-history.csv — Monthly operating history from the property-management system

month | rooms_available | rooms_sold | adr | revpar | room_revenue | fb_revenue | gross_operating_profit
2024-10 | 5400 | 3488 | 134.71 | 87.01 | 469871.27 | 89275.54 | 159756.23
2024-11 | 5400 | 2937 | 132.72 | 72.18 | 389798.64 | 74061.74 | 132531.54
2024-12 | 5400 | 2864 | 132.45 | 70.25 | 379349.86 | 72076.47 | 128978.95
2025-01 | 5400 | 2643 | 131.66 | 64.44 | 347972.73 | 66114.82 | 118310.73
2025-02 | 5400 | 2790 | 132.19 | 68.30 | 368807.64 | 70073.45 | 125394.60
2025-03 | 5400 | 3084 | 133.25 | 76.10 | 410945.71 | 78079.68 | 139721.54
2025-04 | 5400 | 3304 | 134.05 | 82.02 | 442891.95 | 84149.47 | 150583.26
2025-05 | 5400 | 3672 | 135.37 | 92.05 | 497094.80 | 94448.01 | 169012.23
2025-06 | 5400 | 4332 | 137.76 | 110.52 | 596790.88 | 113390.27 | 202908.90
2025-07 | 5400 | 4847 | 139.62 | 125.32 | 676745.12 | 128581.57 | 230093.34
2025-08 | 5400 | 4773 | 139.36 | 123.18 | 665146.19 | 126377.78 | 226149.70
2025-09 | 5400 | 3965 | 136.44 | 100.18 | 540969.37 | 102784.18 | 183929.59
2025-10 | 5400 | 3488 | 136.73 | 88.32 | 476919.34 | 90614.67 | 162152.58
2025-11 | 5400 | 2937 | 134.71 | 73.27 | 395645.62 | 75172.67 | 134519.51
2025-12 | 5400 | 2864 | 134.44 | 71.30 | 385040.11 | 73157.62 | 130913.64
2026-01 | 5400 | 2643 | 133.63 | 65.41 | 353192.32 | 67106.54 | 120085.39
2026-02 | 5400 | 2790 | 134.17 | 69.32 | 374339.76 | 71124.55 | 127275.52
2026-03 | 5400 | 3084 | 135.25 | 77.24 | 417109.90 | 79250.88 | 141817.37
2026-04 | 5400 | 3304 | 136.06 | 83.25 | 449535.33 | 85411.71 | 152842.01
2026-05 | 5400 | 3672 | 137.41 | 93.44 | 504551.22 | 95864.73 | 171547.41
2026-06 | 5400 | 4332 | 139.83 | 112.17 | 605742.74 | 115091.12 | 205952.53
2026-07 | 5400 | 4847 | 141.72 | 127.20 | 686896.30 | 130510.30 | 233544.74
2026-08 | 5400 | 4773 | 141.45 | 125.02 | 675123.38 | 128273.44 | 229541.95
2026-09 | 5400 | 3965 | 138.48 | 101.68 | 549083.92 | 104325.94 | 186688.53
---page---
str-benchmark.csv — STR benchmark report against the competitive set, by month

month | occupancy | adr | revpar | comp_set_revpar
2025-10 | 0.646 | 136.73 | 88.32 | 89.20
2025-11 | 0.544 | 134.71 | 73.27 | 74.30
2025-12 | 0.530 | 134.44 | 71.30 | 72.59
2026-01 | 0.490 | 133.63 | 65.41 | 66.86
2026-02 | 0.517 | 134.17 | 69.32 | 71.14
2026-03 | 0.571 | 135.25 | 77.24 | 79.59
2026-04 | 0.612 | 136.06 | 83.25 | 86.12
2026-05 | 0.680 | 137.41 | 93.44 | 97.05
2026-06 | 0.802 | 139.83 | 112.17 | 116.97
2026-07 | 0.898 | 141.72 | 127.20 | 133.17
2026-08 | 0.884 | 141.45 | 125.02 | 131.41
2026-09 | 0.734 | 138.48 | 101.68 | 107.31
---page---
agreements-register.csv — Agreements register: the franchise and management agreements’ term, fees and early-termination penalty

agreement_id | kind | counterparty | effective_on | expires_on | fee_rate | other_fee_rate | termination_fee
MER-2009 | franchise | Meridale Hotels (synthetic) | 2009-12-01 | 2029-12-31 | 0.055 | 0.044 | 2133000.00
CHM-2019 | management | Coastline Hospitality Management (synthetic) | 2019-01-01 | 2034-12-31 | 0.03 | 0.10 | 
---page---
pip-schedule.csv — The brand’s property improvement plan: items, estimated cost and due dates

item_id | area | description | estimated_cost | due_on
PIP-01 | Guestrooms | Replace guestroom soft goods and casegoods to the current brand standard | 1185000.00 | 2027-06-30
PIP-02 | Public areas | Renovate the lobby, bar and meeting rooms | 711000.00 | 2027-09-30
PIP-03 | Exterior | Replace exterior signage and the porte-cochère canopy | 316000.00 | 2028-06-30
PIP-04 | Guestrooms | Refit guest bathrooms with walk-in showers | 632000.00 | 2028-12-31
---page---
capex-budget.csv — The owner’s capital expenditure budget, FY2027 and FY2028, each line naming the PIP item it funds

fiscal_year | line | pip_ref | amount
2027 | Lobby, bar and meeting room renovation | PIP-02 | 711000.00
2027 | Roof membrane replacement |  | 276500.00
2027 | Kitchen equipment |  | 142200.00
2028 | Exterior signage and canopy | PIP-03 | 316000.00
2028 | Lift modernisation |  | 205400.00
---page---
pnl.csv — Profit and loss by calendar year, FY2021 to FY2025

Line | FY2021 | FY2022 | FY2023 | FY2024 | FY2025
Rooms revenue | 5469350.68 | 5551390.95 | 5634661.79 | 5719181.73 | 5804969.46
Food and beverage revenue | 1039176.63 | 1054764.27 | 1070585.73 | 1086644.52 | 1102944.19
Other operating revenue | 273467.53 | 277569.55 | 281733.09 | 285959.09 | 290248.47
Cost of rooms department | 1312644.16 | 1332333.83 | 1352318.83 | 1372603.62 | 1393192.67
Cost of food and beverage | 727423.64 | 738334.99 | 749410.01 | 760651.16 | 772060.93
Franchise and brand fees | 410201.30 | 444111.28 | 484580.91 | 526164.72 | 574691.98
Management fees | 203459.85 | 206511.74 | 209609.42 | 212753.56 | 215944.86
Utilities and energy | 305189.77 | 309767.61 | 314414.13 | 319130.34 | 323917.30
Repairs and maintenance | 271279.79 | 275348.99 | 279479.22 | 283671.41 | 287926.48
General and administrative | 610379.54 | 619535.23 | 628828.25 | 638260.68 | 647834.59
