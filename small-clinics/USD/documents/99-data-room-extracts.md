Clearbrook Clinics Inc. — data-room extracts (synthetic demo data)

Each page reproduces one structured extract from this folder. All names and figures are fictional.
---page---
patient-volume.csv — Visits and revenue by site and pseudonymous provider

month | site | provider_ref | visits | revenue
2025-10 | Site 1 | P01 | 147 | 15435.00
2025-10 | Site 1 | P02 | 150 | 15750.00
2025-10 | Site 1 | P03 | 196 | 20580.00
2025-10 | Site 1 | P04 | 168 | 17640.00
2025-10 | Site 2 | P05 | 195 | 20475.00
2025-10 | Site 2 | P06 | 136 | 14280.00
2025-10 | Site 2 | P07 | 183 | 19215.00
2025-10 | Site 2 | P08 | 184 | 19320.00
2025-10 | Site 3 | P07 | 240 | 25200.00
2025-10 | Site 3 | P08 | 85 | 8925.00
2025-10 | Site 4 | P13 | 149 | 15645.00
2025-10 | Site 4 | P14 | 192 | 20160.00
2025-10 | Site 4 | P15 | 194 | 20370.00
2025-10 | Site 4 | P16 | 140 | 14700.00
2025-10 | Site 5 | P17 | 142 | 14910.00
2025-10 | Site 5 | P18 | 172 | 18060.00
2025-10 | Site 5 | P19 | 120 | 12600.00
2025-10 | Site 5 | P20 | 156 | 16380.00
2025-10 | Site 6 | P21 | 193 | 20265.00
2025-10 | Site 6 | P22 | 196 | 20580.00
2025-10 | Site 6 | P23 | 131 | 13755.00
2025-10 | Site 6 | P24 | 180 | 18900.00
2025-11 | Site 1 | P01 | 173 | 18165.00
2025-11 | Site 1 | P02 | 145 | 15225.00
2025-11 | Site 1 | P03 | 148 | 15540.00
2025-11 | Site 1 | P04 | 160 | 16800.00
2025-11 | Site 2 | P05 | 180 | 18900.00
2025-11 | Site 2 | P06 | 177 | 18585.00
2025-11 | Site 2 | P07 | 165 | 17325.00
2025-11 | Site 2 | P08 | 149 | 15645.00
2025-11 | Site 3 | P07 | 240 | 25200.00
2025-11 | Site 3 | P08 | 85 | 8925.00
2025-11 | Site 4 | P13 | 182 | 19110.00
2025-11 | Site 4 | P14 | 197 | 20685.00
2025-11 | Site 4 | P15 | 197 | 20685.00
2025-11 | Site 4 | P16 | 149 | 15645.00
2025-11 | Site 5 | P17 | 142 | 14910.00
2025-11 | Site 5 | P18 | 185 | 19425.00
2025-11 | Site 5 | P19 | 132 | 13860.00
2025-11 | Site 5 | P20 | 128 | 13440.00
2025-11 | Site 6 | P21 | 144 | 15120.00
2025-11 | Site 6 | P22 | 130 | 13650.00
2025-11 | Site 6 | P23 | 141 | 14805.00
2025-11 | Site 6 | P24 | 129 | 13545.00
2025-12 | Site 1 | P01 | 176 | 18480.00
2025-12 | Site 1 | P02 | 198 | 20790.00
2025-12 | Site 1 | P03 | 169 | 17745.00
2025-12 | Site 1 | P04 | 197 | 20685.00
2025-12 | Site 2 | P05 | 180 | 18900.00
2025-12 | Site 2 | P06 | 199 | 20895.00
2025-12 | Site 2 | P07 | 164 | 17220.00
2025-12 | Site 2 | P08 | 187 | 19635.00
2025-12 | Site 3 | P07 | 240 | 25200.00
2025-12 | Site 3 | P08 | 85 | 8925.00
2025-12 | Site 4 | P13 | 132 | 13860.00
2025-12 | Site 4 | P14 | 188 | 19740.00
2025-12 | Site 4 | P15 | 165 | 17325.00
2025-12 | Site 4 | P16 | 151 | 15855.00
2025-12 | Site 5 | P17 | 184 | 19320.00
2025-12 | Site 5 | P18 | 198 | 20790.00
… 204 more rows in patient-volume.csv
---page---
equipment-schedule.csv — Equipment with acquisition dates and useful lives

asset | site | acquired | useful_life_years | status
Panoramic X-ray unit | Site 1 | 2014-05-01 | 10 | in service
Panoramic X-ray unit | Site 4 | 2015-02-01 | 10 | in service
Dental chairs (6) | Site 2 | 2021-09-01 | 12 | in service
Shockwave therapy unit | Site 5 | 2023-03-01 | 8 | in service
---page---
coding-summary.csv — Share of visits billed at the highest complexity code

quarter | high_complexity_share | policy_benchmark
2025-Q4 | 0.31 | 0.15
2026-Q1 | 0.33 | 0.15
2026-Q2 | 0.34 | 0.15
2026-Q3 | 0.36 | 0.15
---page---
remittances.csv — Remittances by month and payer: claims, denials, charges billed, cash collected and receivables at month end

month | payer | payer_class | claims | denied_claims | billed | collected | ar_balance
2023-01 | Insurer Bluepoint (synthetic) | commercial | 746 | 36 | 114817.35 | 87646.83 | 135424.04
2023-01 | Insurer Harrowgate (synthetic) | commercial | 426 | 20 | 65349.23 | 49884.91 | 77000.31
2023-01 | Government scheme (synthetic) | medicaid | 502 | 24 | 48180.44 | 36778.96 | 57569.29
2023-01 | Patients — self-pay (synthetic) | self_pay | 360 | 17 | 44897.13 | 34272.62 | 53167.65
2023-02 | Insurer Bluepoint (synthetic) | commercial | 749 | 36 | 115391.44 | 88085.07 | 135964.52
2023-02 | Insurer Harrowgate (synthetic) | commercial | 424 | 20 | 65675.97 | 50134.33 | 76918.66
2023-02 | Government scheme (synthetic) | medicaid | 502 | 24 | 48421.35 | 36962.86 | 57169.05
2023-02 | Patients — self-pay (synthetic) | self_pay | 361 | 17 | 45121.61 | 34443.98 | 53647.22
2023-03 | Insurer Bluepoint (synthetic) | commercial | 744 | 35 | 115968.39 | 88525.49 | 136644.33
2023-03 | Insurer Harrowgate (synthetic) | commercial | 429 | 20 | 66004.35 | 50385.00 | 79257.33
2023-03 | Government scheme (synthetic) | medicaid | 500 | 24 | 48663.45 | 37147.67 | 56820.98
2023-03 | Patients — self-pay (synthetic) | self_pay | 357 | 17 | 45347.22 | 34616.20 | 53700.66
2023-04 | Insurer Bluepoint (synthetic) | commercial | 747 | 36 | 116548.24 | 88968.12 | 136775.49
2023-04 | Insurer Harrowgate (synthetic) | commercial | 425 | 20 | 66334.38 | 50636.93 | 79182.30
2023-04 | Government scheme (synthetic) | medicaid | 505 | 25 | 48906.77 | 37333.41 | 58263.41
2023-04 | Patients — self-pay (synthetic) | self_pay | 359 | 17 | 45573.96 | 34789.28 | 54346.95
2023-05 | Insurer Bluepoint (synthetic) | commercial | 763 | 38 | 117130.98 | 89412.96 | 137875.49
2023-05 | Insurer Harrowgate (synthetic) | commercial | 430 | 21 | 66666.04 | 50890.11 | 80130.83
2023-05 | Government scheme (synthetic) | medicaid | 511 | 24 | 49151.30 | 37520.08 | 58554.72
2023-05 | Patients — self-pay (synthetic) | self_pay | 361 | 18 | 45801.83 | 34963.23 | 54076.29
2023-06 | Insurer Bluepoint (synthetic) | commercial | 766 | 38 | 117716.63 | 89860.02 | 139261.87
2023-06 | Insurer Harrowgate (synthetic) | commercial | 430 | 21 | 66999.37 | 51144.56 | 78944.65
2023-06 | Government scheme (synthetic) | medicaid | 511 | 25 | 49397.06 | 37707.68 | 58145.54
2023-06 | Patients — self-pay (synthetic) | self_pay | 363 | 17 | 46030.83 | 35138.04 | 54891.76
2023-07 | Insurer Bluepoint (synthetic) | commercial | 762 | 37 | 118305.21 | 90309.32 | 140658.67
2023-07 | Insurer Harrowgate (synthetic) | commercial | 438 | 21 | 67334.38 | 51400.29 | 80455.72
2023-07 | Government scheme (synthetic) | medicaid | 512 | 24 | 49644.05 | 37896.22 | 59670.84
2023-07 | Patients — self-pay (synthetic) | self_pay | 370 | 18 | 46260.99 | 35313.73 | 55111.45
2023-08 | Insurer Bluepoint (synthetic) | commercial | 766 | 36 | 118896.74 | 90760.87 | 141643.56
2023-08 | Insurer Harrowgate (synthetic) | commercial | 440 | 22 | 67671.05 | 51657.29 | 80216.91
2023-08 | Government scheme (synthetic) | medicaid | 511 | 24 | 49892.27 | 38085.70 | 59437.45
2023-08 | Patients — self-pay (synthetic) | self_pay | 368 | 18 | 46492.29 | 35490.30 | 54340.92
2023-09 | Insurer Bluepoint (synthetic) | commercial | 768 | 37 | 119491.23 | 91214.68 | 141361.27
2023-09 | Insurer Harrowgate (synthetic) | commercial | 442 | 22 | 68009.40 | 51915.57 | 80698.52
2023-09 | Government scheme (synthetic) | medicaid | 522 | 25 | 50141.73 | 38276.13 | 58784.58
2023-09 | Patients — self-pay (synthetic) | self_pay | 370 | 18 | 46724.75 | 35667.75 | 54612.63
2023-10 | Insurer Bluepoint (synthetic) | commercial | 772 | 37 | 120088.68 | 91670.75 | 140788.18
2023-10 | Insurer Harrowgate (synthetic) | commercial | 445 | 22 | 68349.45 | 52175.15 | 80130.74
2023-10 | Government scheme (synthetic) | medicaid | 525 | 26 | 50392.44 | 38467.51 | 58780.13
2023-10 | Patients — self-pay (synthetic) | self_pay | 376 | 18 | 46958.38 | 35846.09 | 55274.96
2023-11 | Insurer Bluepoint (synthetic) | commercial | 780 | 37 | 120689.12 | 92129.10 | 143778.85
2023-11 | Insurer Harrowgate (synthetic) | commercial | 449 | 22 | 68691.20 | 52436.03 | 80938.12
2023-11 | Government scheme (synthetic) | medicaid | 524 | 25 | 50644.40 | 38659.85 | 59373.90
2023-11 | Patients — self-pay (synthetic) | self_pay | 375 | 18 | 47193.17 | 36025.32 | 55271.90
2023-12 | Insurer Bluepoint (synthetic) | commercial | 787 | 39 | 121292.57 | 92589.75 | 144785.03
2023-12 | Insurer Harrowgate (synthetic) | commercial | 442 | 21 | 69034.66 | 52698.21 | 80852.30
2023-12 | Government scheme (synthetic) | medicaid | 525 | 25 | 50897.63 | 38853.15 | 60695.42
2023-12 | Patients — self-pay (synthetic) | self_pay | 379 | 18 | 47429.14 | 36205.45 | 56390.75
2024-01 | Insurer Bluepoint (synthetic) | commercial | 787 | 37 | 121899.04 | 93052.70 | 146375.08
2024-01 | Insurer Harrowgate (synthetic) | commercial | 445 | 21 | 69379.83 | 52961.70 | 81338.72
2024-01 | Government scheme (synthetic) | medicaid | 522 | 26 | 51152.11 | 39047.41 | 60998.89
2024-01 | Patients — self-pay (synthetic) | self_pay | 379 | 19 | 47666.29 | 36386.48 | 57124.29
2024-02 | Insurer Bluepoint (synthetic) | commercial | 794 | 39 | 122508.53 | 93517.96 | 144640.66
2024-02 | Insurer Harrowgate (synthetic) | commercial | 451 | 21 | 69726.73 | 53226.51 | 82240.84
2024-02 | Government scheme (synthetic) | medicaid | 532 | 26 | 51407.87 | 39242.65 | 61669.15
2024-02 | Patients — self-pay (synthetic) | self_pay | 379 | 19 | 47904.62 | 36568.41 | 56161.86
2024-03 | Insurer Bluepoint (synthetic) | commercial | 789 | 38 | 123121.07 | 93985.55 | 147988.29
2024-03 | Insurer Harrowgate (synthetic) | commercial | 452 | 22 | 70075.36 | 53492.64 | 84228.74
2024-03 | Government scheme (synthetic) | medicaid | 533 | 26 | 51664.91 | 39438.86 | 61304.49
2024-03 | Patients — self-pay (synthetic) | self_pay | 379 | 19 | 48144.14 | 36751.25 | 57411.89
… 120 more rows in remittances.csv
---page---
service-lines.csv — Collections and direct costs by month, service line and pseudonymous provider, from the schedule and billing exports

month | service_line | provider_ref | visits | collected | direct_cost
2025-10 | Implants | P01 | 132 | 40911.98 | 13910.07
2025-10 | Restorative dentistry | P01 | 51 | 6158.03 | 2832.69
2025-10 | Restorative dentistry | P02 | 205 | 24632.12 | 11330.78
2025-10 | Restorative dentistry | P05 | 188 | 22579.45 | 10386.55
2025-10 | Restorative dentistry | P06 | 137 | 16421.42 | 7553.85
2025-10 | Hygiene | P03 | 249 | 21177.96 | 11012.54
2025-10 | Hygiene | P04 | 187 | 15883.47 | 8259.40
2025-10 | Hygiene | P09 | 187 | 15883.48 | 8259.41
2025-10 | Physiotherapy | P13 | 181 | 15402.16 | 8471.19
2025-10 | Physiotherapy | P14 | 181 | 15402.16 | 8471.19
2025-10 | Physiotherapy | P17 | 181 | 15402.16 | 8471.19
2025-10 | Physiotherapy | P18 | 161 | 13690.81 | 7529.95
2025-10 | Physiotherapy | P21 | 201 | 17113.49 | 9412.42
2025-11 | Implants | P01 | 134 | 41582.07 | 14137.90
2025-11 | Restorative dentistry | P01 | 57 | 6864.59 | 3157.71
2025-11 | Restorative dentistry | P02 | 172 | 20593.78 | 9473.14
2025-11 | Restorative dentistry | P05 | 191 | 22881.97 | 10525.71
2025-11 | Restorative dentistry | P06 | 172 | 20593.78 | 9473.14
2025-11 | Hygiene | P03 | 203 | 17219.87 | 8954.33
2025-11 | Hygiene | P04 | 228 | 19372.35 | 10073.62
2025-11 | Hygiene | P09 | 203 | 17219.87 | 8954.33
2025-11 | Physiotherapy | P13 | 221 | 18785.31 | 10331.92
2025-11 | Physiotherapy | P14 | 184 | 15654.42 | 8609.93
2025-11 | Physiotherapy | P17 | 184 | 15654.42 | 8609.93
2025-11 | Physiotherapy | P18 | 147 | 12523.54 | 6887.95
2025-11 | Physiotherapy | P21 | 184 | 15654.43 | 8609.94
2025-12 | Implants | P01 | 135 | 41887.54 | 14241.76
2025-12 | Restorative dentistry | P01 | 53 | 6304.87 | 2900.24
2025-12 | Restorative dentistry | P02 | 140 | 16812.99 | 7733.98
2025-12 | Restorative dentistry | P05 | 210 | 25219.49 | 11600.97
2025-12 | Restorative dentistry | P06 | 193 | 23117.87 | 10634.22
2025-12 | Hygiene | P03 | 226 | 19234.89 | 10002.14
2025-12 | Hygiene | P04 | 226 | 19234.89 | 10002.14
2025-12 | Hygiene | P09 | 185 | 15737.63 | 8183.57
2025-12 | Physiotherapy | P13 | 193 | 16364.50 | 9000.48
2025-12 | Physiotherapy | P14 | 158 | 13389.14 | 7364.03
2025-12 | Physiotherapy | P17 | 175 | 14876.82 | 8182.25
2025-12 | Physiotherapy | P18 | 193 | 16364.50 | 9000.48
2025-12 | Physiotherapy | P21 | 210 | 17852.18 | 9818.70
2026-01 | Implants | P01 | 134 | 41499.99 | 14110.00
2026-01 | Restorative dentistry | P01 | 55 | 6636.95 | 3053.00
2026-01 | Restorative dentistry | P02 | 221 | 26547.78 | 12211.98
2026-01 | Restorative dentistry | P05 | 147 | 17698.52 | 8141.32
2026-01 | Restorative dentistry | P06 | 166 | 19910.84 | 9158.99
2026-01 | Hygiene | P03 | 178 | 15104.77 | 7854.48
2026-01 | Hygiene | P04 | 217 | 18461.39 | 9599.92
2026-01 | Hygiene | P09 | 237 | 20139.70 | 10472.64
2026-01 | Physiotherapy | P13 | 153 | 13019.60 | 7160.78
2026-01 | Physiotherapy | P14 | 211 | 17901.95 | 9846.07
2026-01 | Physiotherapy | P17 | 191 | 16274.50 | 8950.98
2026-01 | Physiotherapy | P18 | 172 | 14647.05 | 8055.88
2026-01 | Physiotherapy | P21 | 191 | 16274.52 | 8950.99
2026-02 | Implants | P01 | 138 | 42867.78 | 14575.05
2026-02 | Restorative dentistry | P01 | 57 | 6855.69 | 3153.62
2026-02 | Restorative dentistry | P02 | 171 | 20567.08 | 9460.86
2026-02 | Restorative dentistry | P05 | 152 | 18281.85 | 8409.65
2026-02 | Restorative dentistry | P06 | 229 | 27422.78 | 12614.48
2026-02 | Hygiene | P03 | 201 | 17069.53 | 8876.16
2026-02 | Hygiene | P04 | 251 | 21336.91 | 11095.19
2026-02 | Hygiene | P09 | 201 | 17069.52 | 8876.15
… 96 more rows in service-lines.csv
---page---
clinician-collections.csv — Collections by clinician and month, pseudonymous, from the practice-management system

month | provider_ref | site | visits | collected
2025-10 | P01 | Site 1 (synthetic) | 183 | 47070.01
2025-10 | P02 | Site 1 (synthetic) | 205 | 24632.12
2025-10 | P03 | Site 1 (synthetic) | 249 | 21177.96
2025-10 | P04 | Site 2 (synthetic) | 187 | 15883.47
2025-10 | P05 | Site 2 (synthetic) | 188 | 22579.45
2025-10 | P06 | Site 4 (synthetic) | 137 | 16421.42
2025-10 | P09 | Site 3 (synthetic) | 187 | 15883.48
2025-10 | P13 | Site 4 (synthetic) | 181 | 15402.16
2025-10 | P14 | Site 5 (synthetic) | 181 | 15402.16
2025-10 | P17 | Site 5 (synthetic) | 181 | 15402.16
2025-10 | P18 | Site 6 (synthetic) | 161 | 13690.81
2025-10 | P21 | Site 6 (synthetic) | 201 | 17113.49
2025-11 | P01 | Site 1 (synthetic) | 191 | 48446.66
2025-11 | P02 | Site 1 (synthetic) | 172 | 20593.78
2025-11 | P03 | Site 1 (synthetic) | 203 | 17219.87
2025-11 | P04 | Site 2 (synthetic) | 228 | 19372.35
2025-11 | P05 | Site 2 (synthetic) | 191 | 22881.97
2025-11 | P06 | Site 4 (synthetic) | 172 | 20593.78
2025-11 | P09 | Site 3 (synthetic) | 203 | 17219.87
2025-11 | P13 | Site 4 (synthetic) | 221 | 18785.31
2025-11 | P14 | Site 5 (synthetic) | 184 | 15654.42
2025-11 | P17 | Site 5 (synthetic) | 184 | 15654.42
2025-11 | P18 | Site 6 (synthetic) | 147 | 12523.54
2025-11 | P21 | Site 6 (synthetic) | 184 | 15654.43
2025-12 | P01 | Site 1 (synthetic) | 188 | 48192.41
2025-12 | P02 | Site 1 (synthetic) | 140 | 16812.99
2025-12 | P03 | Site 1 (synthetic) | 226 | 19234.89
2025-12 | P04 | Site 2 (synthetic) | 226 | 19234.89
2025-12 | P05 | Site 2 (synthetic) | 210 | 25219.49
2025-12 | P06 | Site 4 (synthetic) | 193 | 23117.87
2025-12 | P09 | Site 3 (synthetic) | 185 | 15737.63
2025-12 | P13 | Site 4 (synthetic) | 193 | 16364.50
2025-12 | P14 | Site 5 (synthetic) | 158 | 13389.14
2025-12 | P17 | Site 5 (synthetic) | 175 | 14876.82
2025-12 | P18 | Site 6 (synthetic) | 193 | 16364.50
2025-12 | P21 | Site 6 (synthetic) | 210 | 17852.18
2026-01 | P01 | Site 1 (synthetic) | 189 | 48136.94
2026-01 | P02 | Site 1 (synthetic) | 221 | 26547.78
2026-01 | P03 | Site 1 (synthetic) | 178 | 15104.77
2026-01 | P04 | Site 2 (synthetic) | 217 | 18461.39
2026-01 | P05 | Site 2 (synthetic) | 147 | 17698.52
2026-01 | P06 | Site 4 (synthetic) | 166 | 19910.84
2026-01 | P09 | Site 3 (synthetic) | 237 | 20139.70
2026-01 | P13 | Site 4 (synthetic) | 153 | 13019.60
2026-01 | P14 | Site 5 (synthetic) | 211 | 17901.95
2026-01 | P17 | Site 5 (synthetic) | 191 | 16274.50
2026-01 | P18 | Site 6 (synthetic) | 172 | 14647.05
2026-01 | P21 | Site 6 (synthetic) | 191 | 16274.52
2026-02 | P01 | Site 1 (synthetic) | 195 | 49723.47
2026-02 | P02 | Site 1 (synthetic) | 171 | 20567.08
2026-02 | P03 | Site 1 (synthetic) | 201 | 17069.53
2026-02 | P04 | Site 2 (synthetic) | 251 | 21336.91
2026-02 | P05 | Site 2 (synthetic) | 152 | 18281.85
2026-02 | P06 | Site 4 (synthetic) | 229 | 27422.78
2026-02 | P09 | Site 3 (synthetic) | 201 | 17069.52
2026-02 | P13 | Site 4 (synthetic) | 158 | 13448.72
2026-02 | P14 | Site 5 (synthetic) | 178 | 15129.81
2026-02 | P17 | Site 5 (synthetic) | 178 | 15129.81
2026-02 | P18 | Site 6 (synthetic) | 198 | 16810.90
2026-02 | P21 | Site 6 (synthetic) | 237 | 20173.06
… 84 more rows in clinician-collections.csv
---page---
referrals.csv — Visits by referral source and month, from the schedule export

month | referral_source | source_type | visits | new_patients
2025-10 | Harbourside Hospital orthopaedics (synthetic) | hospital | 677 | 149
2025-10 | Northgate Physician Group (synthetic) | physician group | 152 | 33
2025-10 | Bluepoint plan network (synthetic) | plan | 105 | 23
2025-10 | Self-referral | self-referral | 234 | 51
2025-11 | Harbourside Hospital orthopaedics (synthetic) | hospital | 701 | 154
2025-11 | Northgate Physician Group (synthetic) | physician group | 157 | 35
2025-11 | Bluepoint plan network (synthetic) | plan | 109 | 24
2025-11 | Self-referral | self-referral | 242 | 53
2025-12 | Harbourside Hospital orthopaedics (synthetic) | hospital | 693 | 152
2025-12 | Northgate Physician Group (synthetic) | physician group | 155 | 34
2025-12 | Bluepoint plan network (synthetic) | plan | 108 | 24
2025-12 | Self-referral | self-referral | 239 | 53
2026-01 | Harbourside Hospital orthopaedics (synthetic) | hospital | 677 | 149
2026-01 | Northgate Physician Group (synthetic) | physician group | 152 | 33
2026-01 | Bluepoint plan network (synthetic) | plan | 105 | 23
2026-01 | Self-referral | self-referral | 234 | 51
2026-02 | Harbourside Hospital orthopaedics (synthetic) | hospital | 670 | 147
2026-02 | Northgate Physician Group (synthetic) | physician group | 150 | 33
2026-02 | Bluepoint plan network (synthetic) | plan | 104 | 23
2026-02 | Self-referral | self-referral | 232 | 51
2026-03 | Harbourside Hospital orthopaedics (synthetic) | hospital | 687 | 151
2026-03 | Northgate Physician Group (synthetic) | physician group | 154 | 34
2026-03 | Bluepoint plan network (synthetic) | plan | 107 | 24
2026-03 | Self-referral | self-referral | 236 | 52
2026-04 | Harbourside Hospital orthopaedics (synthetic) | hospital | 691 | 152
2026-04 | Northgate Physician Group (synthetic) | physician group | 155 | 34
2026-04 | Bluepoint plan network (synthetic) | plan | 107 | 24
2026-04 | Self-referral | self-referral | 239 | 53
2026-05 | Harbourside Hospital orthopaedics (synthetic) | hospital | 677 | 149
2026-05 | Northgate Physician Group (synthetic) | physician group | 152 | 33
2026-05 | Bluepoint plan network (synthetic) | plan | 105 | 23
2026-05 | Self-referral | self-referral | 234 | 51
2026-06 | Harbourside Hospital orthopaedics (synthetic) | hospital | 696 | 153
2026-06 | Northgate Physician Group (synthetic) | physician group | 156 | 34
2026-06 | Bluepoint plan network (synthetic) | plan | 108 | 24
2026-06 | Self-referral | self-referral | 240 | 53
2026-07 | Harbourside Hospital orthopaedics (synthetic) | hospital | 680 | 150
2026-07 | Northgate Physician Group (synthetic) | physician group | 152 | 33
2026-07 | Bluepoint plan network (synthetic) | plan | 105 | 23
2026-07 | Self-referral | self-referral | 235 | 52
2026-08 | Harbourside Hospital orthopaedics (synthetic) | hospital | 690 | 152
2026-08 | Northgate Physician Group (synthetic) | physician group | 155 | 34
2026-08 | Bluepoint plan network (synthetic) | plan | 107 | 24
2026-08 | Self-referral | self-referral | 238 | 52
2026-09 | Harbourside Hospital orthopaedics (synthetic) | hospital | 683 | 150
2026-09 | Northgate Physician Group (synthetic) | physician group | 153 | 34
2026-09 | Bluepoint plan network (synthetic) | plan | 106 | 23
2026-09 | Self-referral | self-referral | 235 | 52
---page---
credentialing-register.csv — Credentialing register: a licence per pseudonymous provider

credential_ref | provider_ref | kind | jurisdiction | issuer | status | expires_on
CR-0101 | P01 | state_licence | Ohio | Ohio dental board (synthetic) | active | 2027-01-28
CR-0201 | P02 | state_licence | Ohio | Ohio dental board (synthetic) | active | 2028-02-28
CR-0301 | P03 | state_licence | Ohio | Ohio dental board (synthetic) | active | 2027-03-28
CR-0401 | P04 | state_licence | Ohio | Ohio dental board (synthetic) | active | 2028-04-28
CR-0501 | P05 | state_licence | Ohio | Ohio dental board (synthetic) | active | 2027-05-28
CR-0601 | P06 | state_licence | Ohio | Ohio dental board (synthetic) | active | 2028-06-28
CR-0701 | P09 | state_licence | Ohio | Ohio dental board (synthetic) | active | 2027-07-28
CR-0801 | P13 | state_licence | Ohio | Ohio physiotherapy board (synthetic) | active | 2028-08-28
CR-0901 | P14 | state_licence | Ohio | Ohio physiotherapy board (synthetic) | active | 2027-09-28
CR-1001 | P17 | state_licence | Ohio | Ohio physiotherapy board (synthetic) | active | 2028-10-28
CR-1101 | P18 | state_licence | Ohio | Ohio physiotherapy board (synthetic) | active | 2027-11-28
CR-1201 | P21 | state_licence | Ohio | Ohio physiotherapy board (synthetic) | active | 2028-12-28
---page---
payer-contracts.csv — Payer contract and enrolment register

contract_id | payer | payer_class | effective_on | expires_on | auto_renews
BP-2023 | Insurer Bluepoint (synthetic) | commercial | 2023-01-01 | 2028-12-31 | yes
HG-2024 | Insurer Harrowgate (synthetic) | commercial | 2024-07-01 | 2029-06-30 | no
GS-ENR-118 | Government scheme (synthetic) | medicaid | 2019-04-01 |  | no
---page---
pnl.csv — Profit and loss by fiscal year, FY2023 to FY2025

Line | FY2023 | FY2024 | FY2025
Net patient service revenue | 2572992.55 | 2722434.86 | 2867350.10
Other operating revenue | 9000.00 | 9270.00 | 9540.00
Cost of care: clinical staff | 1058616.95 | 1119998.99 | 1179524.94
Clinical and dental supplies | 175575.49 | 229463.21 | 296319.68
Laboratory fees | 80041.77 | 84682.85 | 86306.70
Rent and occupancy | 191067.45 | 199414.45 | 207136.09
General and administrative | 304675.12 | 281365.60 | 244535.66
