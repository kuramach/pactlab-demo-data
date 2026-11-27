Clearbrook Clinics B.V. — data-room extracts (synthetic demo data)

Each page reproduces one structured extract from this folder. All names and figures are fictional.
---page---
patient-volume.csv — Visits and revenue by site and pseudonymous provider

month | site | provider_ref | visits | revenue
2025-10 | Site 1 | P01 | 159 | 15359.40
2025-10 | Site 1 | P02 | 173 | 16711.80
2025-10 | Site 1 | P03 | 137 | 13234.20
2025-10 | Site 1 | P04 | 130 | 12558.00
2025-10 | Site 2 | P05 | 163 | 15745.80
2025-10 | Site 2 | P06 | 146 | 14103.60
2025-10 | Site 2 | P07 | 131 | 12654.60
2025-10 | Site 2 | P08 | 168 | 16228.80
2025-10 | Site 3 | P07 | 240 | 23184.00
2025-10 | Site 3 | P08 | 85 | 8211.00
2025-10 | Site 4 | P13 | 189 | 18257.40
2025-10 | Site 4 | P14 | 121 | 11688.60
2025-10 | Site 4 | P15 | 122 | 11785.20
2025-10 | Site 4 | P16 | 134 | 12944.40
2025-10 | Site 5 | P17 | 197 | 19030.20
2025-10 | Site 5 | P18 | 139 | 13427.40
2025-10 | Site 5 | P19 | 179 | 17291.40
2025-10 | Site 5 | P20 | 164 | 15842.40
2025-10 | Site 6 | P21 | 153 | 14779.80
2025-10 | Site 6 | P22 | 187 | 18064.20
2025-10 | Site 6 | P23 | 148 | 14296.80
2025-10 | Site 6 | P24 | 184 | 17774.40
2025-11 | Site 1 | P01 | 176 | 17001.60
2025-11 | Site 1 | P02 | 180 | 17388.00
2025-11 | Site 1 | P03 | 137 | 13234.20
2025-11 | Site 1 | P04 | 137 | 13234.20
2025-11 | Site 2 | P05 | 200 | 19320.00
2025-11 | Site 2 | P06 | 126 | 12171.60
2025-11 | Site 2 | P07 | 176 | 17001.60
2025-11 | Site 2 | P08 | 137 | 13234.20
2025-11 | Site 3 | P07 | 240 | 23184.00
2025-11 | Site 3 | P08 | 85 | 8211.00
2025-11 | Site 4 | P13 | 136 | 13137.60
2025-11 | Site 4 | P14 | 155 | 14973.00
2025-11 | Site 4 | P15 | 162 | 15649.20
2025-11 | Site 4 | P16 | 200 | 19320.00
2025-11 | Site 5 | P17 | 166 | 16035.60
2025-11 | Site 5 | P18 | 125 | 12075.00
2025-11 | Site 5 | P19 | 187 | 18064.20
2025-11 | Site 5 | P20 | 164 | 15842.40
2025-11 | Site 6 | P21 | 187 | 18064.20
2025-11 | Site 6 | P22 | 128 | 12364.80
2025-11 | Site 6 | P23 | 148 | 14296.80
2025-11 | Site 6 | P24 | 164 | 15842.40
2025-12 | Site 1 | P01 | 143 | 13813.80
2025-12 | Site 1 | P02 | 148 | 14296.80
2025-12 | Site 1 | P03 | 149 | 14393.40
2025-12 | Site 1 | P04 | 155 | 14973.00
2025-12 | Site 2 | P05 | 127 | 12268.20
2025-12 | Site 2 | P06 | 139 | 13427.40
2025-12 | Site 2 | P07 | 200 | 19320.00
2025-12 | Site 2 | P08 | 147 | 14200.20
2025-12 | Site 3 | P07 | 240 | 23184.00
2025-12 | Site 3 | P08 | 85 | 8211.00
2025-12 | Site 4 | P13 | 159 | 15359.40
2025-12 | Site 4 | P14 | 166 | 16035.60
2025-12 | Site 4 | P15 | 124 | 11978.40
2025-12 | Site 4 | P16 | 134 | 12944.40
2025-12 | Site 5 | P17 | 190 | 18354.00
2025-12 | Site 5 | P18 | 186 | 17967.60
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
2023-01 | Insurer Bluepoint (synthetic) | commercial | 718 | 34 | 101443.36 | 77437.68 | 119409.51
2023-01 | Insurer Harrowgate (synthetic) | commercial | 408 | 19 | 58574.00 | 44712.98 | 68878.40
2023-01 | Government scheme (synthetic) | medicaid | 483 | 23 | 43244.67 | 33011.20 | 50596.26
2023-01 | Patients — self-pay (synthetic) | self_pay | 362 | 17 | 42258.08 | 32258.08 | 50292.68
2023-02 | Insurer Bluepoint (synthetic) | commercial | 719 | 34 | 101950.58 | 77824.87 | 119644.37
2023-02 | Insurer Harrowgate (synthetic) | commercial | 414 | 20 | 58866.88 | 44936.55 | 70617.02
2023-02 | Government scheme (synthetic) | medicaid | 483 | 24 | 43460.90 | 33176.26 | 51930.06
2023-02 | Patients — self-pay (synthetic) | self_pay | 370 | 17 | 42469.37 | 32419.37 | 50141.80
2023-03 | Insurer Bluepoint (synthetic) | commercial | 727 | 36 | 102460.33 | 78213.99 | 121213.27
2023-03 | Insurer Harrowgate (synthetic) | commercial | 412 | 19 | 59161.21 | 45161.23 | 69358.73
2023-03 | Government scheme (synthetic) | medicaid | 492 | 23 | 43678.20 | 33342.14 | 51000.05
2023-03 | Patients — self-pay (synthetic) | self_pay | 365 | 18 | 42681.73 | 32581.47 | 50999.05
2023-04 | Insurer Bluepoint (synthetic) | commercial | 727 | 35 | 102972.63 | 78605.06 | 120234.09
2023-04 | Insurer Harrowgate (synthetic) | commercial | 418 | 20 | 59457.01 | 45387.03 | 69916.75
2023-04 | Government scheme (synthetic) | medicaid | 491 | 23 | 43896.59 | 33508.85 | 52086.77
2023-04 | Patients — self-pay (synthetic) | self_pay | 367 | 17 | 42895.14 | 32744.38 | 50136.52
2023-05 | Insurer Bluepoint (synthetic) | commercial | 726 | 35 | 103487.50 | 78998.09 | 124266.70
2023-05 | Insurer Harrowgate (synthetic) | commercial | 416 | 21 | 59754.30 | 45613.97 | 71186.24
2023-05 | Government scheme (synthetic) | medicaid | 500 | 25 | 44116.07 | 33676.39 | 52242.71
2023-05 | Patients — self-pay (synthetic) | self_pay | 371 | 18 | 43109.61 | 32908.10 | 51459.26
2023-06 | Insurer Bluepoint (synthetic) | commercial | 727 | 35 | 104004.93 | 79393.08 | 124641.70
2023-06 | Insurer Harrowgate (synthetic) | commercial | 418 | 20 | 60053.07 | 45842.04 | 71897.75
2023-06 | Government scheme (synthetic) | medicaid | 498 | 23 | 44336.66 | 33844.78 | 52608.95
2023-06 | Patients — self-pay (synthetic) | self_pay | 373 | 18 | 43325.16 | 33072.64 | 51357.42
2023-07 | Insurer Bluepoint (synthetic) | commercial | 741 | 36 | 104524.95 | 79790.04 | 122294.19
2023-07 | Insurer Harrowgate (synthetic) | commercial | 427 | 21 | 60353.34 | 46071.25 | 71614.00
2023-07 | Government scheme (synthetic) | medicaid | 501 | 24 | 44558.34 | 34014.00 | 53346.89
2023-07 | Patients — self-pay (synthetic) | self_pay | 376 | 18 | 43541.78 | 33238.00 | 50943.88
2023-08 | Insurer Bluepoint (synthetic) | commercial | 742 | 36 | 105047.58 | 80188.99 | 124896.04
2023-08 | Insurer Harrowgate (synthetic) | commercial | 425 | 21 | 60655.11 | 46301.61 | 70750.99
2023-08 | Government scheme (synthetic) | medicaid | 504 | 25 | 44781.13 | 34184.07 | 52446.95
2023-08 | Patients — self-pay (synthetic) | self_pay | 375 | 18 | 43759.49 | 33404.19 | 51094.96
2023-09 | Insurer Bluepoint (synthetic) | commercial | 738 | 36 | 105572.82 | 80589.94 | 123770.24
2023-09 | Insurer Harrowgate (synthetic) | commercial | 432 | 21 | 60958.37 | 46533.11 | 72692.86
2023-09 | Government scheme (synthetic) | medicaid | 509 | 25 | 45005.04 | 34354.99 | 53188.85
2023-09 | Patients — self-pay (synthetic) | self_pay | 380 | 18 | 43978.29 | 33571.21 | 52444.11
2023-10 | Insurer Bluepoint (synthetic) | commercial | 744 | 35 | 106100.69 | 80992.89 | 126650.72
2023-10 | Insurer Harrowgate (synthetic) | commercial | 432 | 21 | 61263.17 | 46765.78 | 73056.33
2023-10 | Government scheme (synthetic) | medicaid | 507 | 24 | 45230.06 | 34526.76 | 53615.48
2023-10 | Patients — self-pay (synthetic) | self_pay | 384 | 18 | 44198.18 | 33739.07 | 52496.97
2023-11 | Insurer Bluepoint (synthetic) | commercial | 755 | 36 | 106631.18 | 81397.85 | 125894.94
2023-11 | Insurer Harrowgate (synthetic) | commercial | 430 | 21 | 61569.49 | 46999.61 | 72400.86
2023-11 | Government scheme (synthetic) | medicaid | 510 | 25 | 45456.21 | 34699.40 | 54314.19
2023-11 | Patients — self-pay (synthetic) | self_pay | 387 | 19 | 44419.17 | 33907.76 | 52759.45
2023-12 | Insurer Bluepoint (synthetic) | commercial | 752 | 37 | 107164.34 | 81804.84 | 128554.91
2023-12 | Insurer Harrowgate (synthetic) | commercial | 437 | 20 | 61877.34 | 47234.61 | 72543.04
2023-12 | Government scheme (synthetic) | medicaid | 515 | 25 | 45683.50 | 34872.90 | 54044.78
2023-12 | Patients — self-pay (synthetic) | self_pay | 382 | 18 | 44641.26 | 34077.30 | 53287.57
2024-01 | Insurer Bluepoint (synthetic) | commercial | 765 | 37 | 107700.16 | 82213.86 | 127539.66
2024-01 | Insurer Harrowgate (synthetic) | commercial | 439 | 22 | 62186.72 | 47470.78 | 74304.95
2024-01 | Government scheme (synthetic) | medicaid | 514 | 24 | 45911.91 | 35047.26 | 55184.91
2024-01 | Patients — self-pay (synthetic) | self_pay | 387 | 18 | 44864.47 | 34247.69 | 53872.78
2024-02 | Insurer Bluepoint (synthetic) | commercial | 768 | 36 | 108238.66 | 82624.93 | 128305.54
2024-02 | Insurer Harrowgate (synthetic) | commercial | 443 | 21 | 62497.65 | 47708.13 | 75046.52
2024-02 | Government scheme (synthetic) | medicaid | 521 | 25 | 46141.48 | 35222.50 | 54368.02
2024-02 | Patients — self-pay (synthetic) | self_pay | 394 | 18 | 45088.80 | 34418.93 | 54088.76
2024-03 | Insurer Bluepoint (synthetic) | commercial | 771 | 37 | 108779.86 | 83038.06 | 127530.07
2024-03 | Insurer Harrowgate (synthetic) | commercial | 443 | 21 | 62810.14 | 47946.67 | 74157.29
2024-03 | Government scheme (synthetic) | medicaid | 524 | 24 | 46372.18 | 35398.61 | 55298.82
2024-03 | Patients — self-pay (synthetic) | self_pay | 396 | 19 | 45314.24 | 34591.02 | 53232.31
… 120 more rows in remittances.csv
---page---
service-lines.csv — Collections and direct costs by month, service line and pseudonymous provider, from the schedule and billing exports

month | service_line | provider_ref | visits | collected | direct_cost
2025-10 | Implants | P01 | 133 | 37891.08 | 12882.97
2025-10 | Restorative dentistry | P01 | 57 | 6255.26 | 2877.42
2025-10 | Restorative dentistry | P02 | 189 | 20850.88 | 9591.40
2025-10 | Restorative dentistry | P05 | 170 | 18765.79 | 8632.26
2025-10 | Restorative dentistry | P06 | 170 | 18765.79 | 8632.26
2025-10 | Hygiene | P03 | 230 | 17979.69 | 9349.44
2025-10 | Hygiene | P04 | 209 | 16345.17 | 8499.49
2025-10 | Hygiene | P09 | 188 | 14710.65 | 7649.54
2025-10 | Physiotherapy | P13 | 169 | 13208.22 | 7264.52
2025-10 | Physiotherapy | P14 | 169 | 13208.22 | 7264.52
2025-10 | Physiotherapy | P17 | 203 | 15849.86 | 8717.42
2025-10 | Physiotherapy | P18 | 203 | 15849.86 | 8717.42
2025-10 | Physiotherapy | P21 | 169 | 13208.21 | 7264.52
2025-11 | Implants | P01 | 135 | 38427.57 | 13065.37
2025-11 | Restorative dentistry | P01 | 57 | 6343.83 | 2918.16
2025-11 | Restorative dentistry | P02 | 172 | 19031.49 | 8754.49
2025-11 | Restorative dentistry | P05 | 172 | 19031.49 | 8754.49
2025-11 | Restorative dentistry | P06 | 192 | 21146.10 | 9727.21
2025-11 | Hygiene | P03 | 220 | 17214.16 | 8951.36
2025-11 | Hygiene | P04 | 196 | 15301.47 | 7956.76
2025-11 | Hygiene | P09 | 220 | 17214.16 | 8951.36
2025-11 | Physiotherapy | P13 | 196 | 15301.48 | 8415.81
2025-11 | Physiotherapy | P14 | 160 | 12519.39 | 6885.66
2025-11 | Physiotherapy | P17 | 196 | 15301.48 | 8415.81
2025-11 | Physiotherapy | P18 | 196 | 15301.48 | 8415.81
2025-11 | Physiotherapy | P21 | 178 | 13910.42 | 7650.73
2025-12 | Implants | P01 | 135 | 38604.61 | 13125.57
2025-12 | Restorative dentistry | P01 | 51 | 5644.71 | 2596.57
2025-12 | Restorative dentistry | P02 | 187 | 20697.26 | 9520.74
2025-12 | Restorative dentistry | P05 | 153 | 16934.12 | 7789.70
2025-12 | Restorative dentistry | P06 | 205 | 22578.84 | 10386.27
2025-12 | Hygiene | P03 | 185 | 14504.20 | 7542.18
2025-12 | Hygiene | P04 | 206 | 16115.78 | 8380.21
2025-12 | Hygiene | P09 | 247 | 19338.93 | 10056.24
2025-12 | Physiotherapy | P13 | 199 | 15571.61 | 8564.39
2025-12 | Physiotherapy | P14 | 166 | 12976.34 | 7136.99
2025-12 | Physiotherapy | P17 | 199 | 15571.61 | 8564.39
2025-12 | Physiotherapy | P18 | 199 | 15571.61 | 8564.39
2025-12 | Physiotherapy | P21 | 166 | 12976.34 | 7136.99
2026-01 | Implants | P01 | 137 | 39118.07 | 13300.14
2026-01 | Restorative dentistry | P01 | 58 | 6457.82 | 2970.60
2026-01 | Restorative dentistry | P02 | 175 | 19373.46 | 8911.79
2026-01 | Restorative dentistry | P05 | 175 | 19373.46 | 8911.79
2026-01 | Restorative dentistry | P06 | 195 | 21526.08 | 9902.00
2026-01 | Hygiene | P03 | 209 | 16330.12 | 8491.66
2026-01 | Hygiene | P04 | 251 | 19596.15 | 10190.00
2026-01 | Hygiene | P09 | 188 | 14697.11 | 7642.50
2026-01 | Physiotherapy | P13 | 169 | 13254.12 | 7289.77
2026-01 | Physiotherapy | P14 | 188 | 14726.80 | 8099.74
2026-01 | Physiotherapy | P17 | 188 | 14726.80 | 8099.74
2026-01 | Physiotherapy | P18 | 226 | 17672.16 | 9719.69
2026-01 | Physiotherapy | P21 | 169 | 13254.12 | 7289.77
2026-02 | Implants | P01 | 135 | 38533.20 | 13101.29
2026-02 | Restorative dentistry | P01 | 50 | 5477.76 | 2519.77
2026-02 | Restorative dentistry | P02 | 198 | 21911.03 | 10079.07
2026-02 | Restorative dentistry | P05 | 182 | 20085.11 | 9239.15
2026-02 | Restorative dentistry | P06 | 165 | 18259.20 | 8399.23
2026-02 | Hygiene | P03 | 236 | 18469.07 | 9603.92
2026-02 | Hygiene | P04 | 189 | 14775.26 | 7683.14
2026-02 | Hygiene | P09 | 213 | 16622.16 | 8643.52
… 96 more rows in service-lines.csv
---page---
clinician-collections.csv — Collections by clinician and month, pseudonymous, from the practice-management system

month | provider_ref | site | visits | collected
2025-10 | P01 | Site 1 (synthetic) | 190 | 44146.34
2025-10 | P02 | Site 1 (synthetic) | 189 | 20850.88
2025-10 | P03 | Site 1 (synthetic) | 230 | 17979.69
2025-10 | P04 | Site 2 (synthetic) | 209 | 16345.17
2025-10 | P05 | Site 2 (synthetic) | 170 | 18765.79
2025-10 | P06 | Site 4 (synthetic) | 170 | 18765.79
2025-10 | P09 | Site 3 (synthetic) | 188 | 14710.65
2025-10 | P13 | Site 4 (synthetic) | 169 | 13208.22
2025-10 | P14 | Site 5 (synthetic) | 169 | 13208.22
2025-10 | P17 | Site 5 (synthetic) | 203 | 15849.86
2025-10 | P18 | Site 6 (synthetic) | 203 | 15849.86
2025-10 | P21 | Site 6 (synthetic) | 169 | 13208.21
2025-11 | P01 | Site 1 (synthetic) | 192 | 44771.40
2025-11 | P02 | Site 1 (synthetic) | 172 | 19031.49
2025-11 | P03 | Site 1 (synthetic) | 220 | 17214.16
2025-11 | P04 | Site 2 (synthetic) | 196 | 15301.47
2025-11 | P05 | Site 2 (synthetic) | 172 | 19031.49
2025-11 | P06 | Site 4 (synthetic) | 192 | 21146.10
2025-11 | P09 | Site 3 (synthetic) | 220 | 17214.16
2025-11 | P13 | Site 4 (synthetic) | 196 | 15301.48
2025-11 | P14 | Site 5 (synthetic) | 160 | 12519.39
2025-11 | P17 | Site 5 (synthetic) | 196 | 15301.48
2025-11 | P18 | Site 6 (synthetic) | 196 | 15301.48
2025-11 | P21 | Site 6 (synthetic) | 178 | 13910.42
2025-12 | P01 | Site 1 (synthetic) | 186 | 44249.32
2025-12 | P02 | Site 1 (synthetic) | 187 | 20697.26
2025-12 | P03 | Site 1 (synthetic) | 185 | 14504.20
2025-12 | P04 | Site 2 (synthetic) | 206 | 16115.78
2025-12 | P05 | Site 2 (synthetic) | 153 | 16934.12
2025-12 | P06 | Site 4 (synthetic) | 205 | 22578.84
2025-12 | P09 | Site 3 (synthetic) | 247 | 19338.93
2025-12 | P13 | Site 4 (synthetic) | 199 | 15571.61
2025-12 | P14 | Site 5 (synthetic) | 166 | 12976.34
2025-12 | P17 | Site 5 (synthetic) | 199 | 15571.61
2025-12 | P18 | Site 6 (synthetic) | 199 | 15571.61
2025-12 | P21 | Site 6 (synthetic) | 166 | 12976.34
2026-01 | P01 | Site 1 (synthetic) | 195 | 45575.89
2026-01 | P02 | Site 1 (synthetic) | 175 | 19373.46
2026-01 | P03 | Site 1 (synthetic) | 209 | 16330.12
2026-01 | P04 | Site 2 (synthetic) | 251 | 19596.15
2026-01 | P05 | Site 2 (synthetic) | 175 | 19373.46
2026-01 | P06 | Site 4 (synthetic) | 195 | 21526.08
2026-01 | P09 | Site 3 (synthetic) | 188 | 14697.11
2026-01 | P13 | Site 4 (synthetic) | 169 | 13254.12
2026-01 | P14 | Site 5 (synthetic) | 188 | 14726.80
2026-01 | P17 | Site 5 (synthetic) | 188 | 14726.80
2026-01 | P18 | Site 6 (synthetic) | 226 | 17672.16
2026-01 | P21 | Site 6 (synthetic) | 169 | 13254.12
2026-02 | P01 | Site 1 (synthetic) | 185 | 44010.96
2026-02 | P02 | Site 1 (synthetic) | 198 | 21911.03
2026-02 | P03 | Site 1 (synthetic) | 236 | 18469.07
2026-02 | P04 | Site 2 (synthetic) | 189 | 14775.26
2026-02 | P05 | Site 2 (synthetic) | 182 | 20085.11
2026-02 | P06 | Site 4 (synthetic) | 165 | 18259.20
2026-02 | P09 | Site 3 (synthetic) | 213 | 16622.16
2026-02 | P13 | Site 4 (synthetic) | 186 | 14506.62
2026-02 | P14 | Site 5 (synthetic) | 204 | 15957.28
2026-02 | P17 | Site 5 (synthetic) | 167 | 13055.95
2026-02 | P18 | Site 6 (synthetic) | 148 | 11605.29
2026-02 | P21 | Site 6 (synthetic) | 223 | 17407.94
… 84 more rows in clinician-collections.csv
---page---
referrals.csv — Visits by referral source and month, from the schedule export

month | referral_source | source_type | visits | new_patients
2025-10 | Harbourside Hospital orthopaedics (synthetic) | hospital | 694 | 153
2025-10 | Northgate Physician Group (synthetic) | physician group | 156 | 34
2025-10 | Bluepoint plan network (synthetic) | plan | 108 | 24
2025-10 | Self-referral | self-referral | 239 | 53
2025-11 | Harbourside Hospital orthopaedics (synthetic) | hospital | 662 | 146
2025-11 | Northgate Physician Group (synthetic) | physician group | 148 | 33
2025-11 | Bluepoint plan network (synthetic) | plan | 103 | 23
2025-11 | Self-referral | self-referral | 228 | 50
2025-12 | Harbourside Hospital orthopaedics (synthetic) | hospital | 706 | 155
2025-12 | Northgate Physician Group (synthetic) | physician group | 158 | 35
2025-12 | Bluepoint plan network (synthetic) | plan | 110 | 24
2025-12 | Self-referral | self-referral | 243 | 53
2026-01 | Harbourside Hospital orthopaedics (synthetic) | hospital | 662 | 146
2026-01 | Northgate Physician Group (synthetic) | physician group | 148 | 33
2026-01 | Bluepoint plan network (synthetic) | plan | 103 | 23
2026-01 | Self-referral | self-referral | 229 | 50
2026-02 | Harbourside Hospital orthopaedics (synthetic) | hospital | 694 | 153
2026-02 | Northgate Physician Group (synthetic) | physician group | 156 | 34
2026-02 | Bluepoint plan network (synthetic) | plan | 108 | 24
2026-02 | Self-referral | self-referral | 239 | 53
2026-03 | Harbourside Hospital orthopaedics (synthetic) | hospital | 677 | 149
2026-03 | Northgate Physician Group (synthetic) | physician group | 152 | 33
2026-03 | Bluepoint plan network (synthetic) | plan | 105 | 23
2026-03 | Self-referral | self-referral | 233 | 51
2026-04 | Harbourside Hospital orthopaedics (synthetic) | hospital | 702 | 154
2026-04 | Northgate Physician Group (synthetic) | physician group | 157 | 35
2026-04 | Bluepoint plan network (synthetic) | plan | 109 | 24
2026-04 | Self-referral | self-referral | 242 | 53
2026-05 | Harbourside Hospital orthopaedics (synthetic) | hospital | 666 | 147
2026-05 | Northgate Physician Group (synthetic) | physician group | 149 | 33
2026-05 | Bluepoint plan network (synthetic) | plan | 103 | 23
2026-05 | Self-referral | self-referral | 231 | 51
2026-06 | Harbourside Hospital orthopaedics (synthetic) | hospital | 684 | 150
2026-06 | Northgate Physician Group (synthetic) | physician group | 153 | 34
2026-06 | Bluepoint plan network (synthetic) | plan | 106 | 23
2026-06 | Self-referral | self-referral | 236 | 52
2026-07 | Harbourside Hospital orthopaedics (synthetic) | hospital | 698 | 154
2026-07 | Northgate Physician Group (synthetic) | physician group | 157 | 35
2026-07 | Bluepoint plan network (synthetic) | plan | 108 | 24
2026-07 | Self-referral | self-referral | 241 | 53
2026-08 | Harbourside Hospital orthopaedics (synthetic) | hospital | 677 | 149
2026-08 | Northgate Physician Group (synthetic) | physician group | 152 | 33
2026-08 | Bluepoint plan network (synthetic) | plan | 105 | 23
2026-08 | Self-referral | self-referral | 233 | 51
2026-09 | Harbourside Hospital orthopaedics (synthetic) | hospital | 665 | 146
2026-09 | Northgate Physician Group (synthetic) | physician group | 149 | 33
2026-09 | Bluepoint plan network (synthetic) | plan | 103 | 23
2026-09 | Self-referral | self-referral | 229 | 50
---page---
credentialing-register.csv — Credentialing register: a licence per pseudonymous provider

credential_ref | provider_ref | kind | jurisdiction | issuer | status | expires_on
CR-0101 | P01 | state_licence | Netherlands | Netherlands dental board (synthetic) | active | 2027-01-28
CR-0201 | P02 | state_licence | Netherlands | Netherlands dental board (synthetic) | active | 2028-02-28
CR-0301 | P03 | state_licence | Netherlands | Netherlands dental board (synthetic) | active | 2027-03-28
CR-0401 | P04 | state_licence | Netherlands | Netherlands dental board (synthetic) | active | 2028-04-28
CR-0501 | P05 | state_licence | Netherlands | Netherlands dental board (synthetic) | active | 2027-05-28
CR-0601 | P06 | state_licence | Netherlands | Netherlands dental board (synthetic) | active | 2028-06-28
CR-0701 | P09 | state_licence | Netherlands | Netherlands dental board (synthetic) | active | 2027-07-28
CR-0801 | P13 | state_licence | Netherlands | Netherlands physiotherapy board (synthetic) | active | 2028-08-28
CR-0901 | P14 | state_licence | Netherlands | Netherlands physiotherapy board (synthetic) | active | 2027-09-28
CR-1001 | P17 | state_licence | Netherlands | Netherlands physiotherapy board (synthetic) | active | 2028-10-28
CR-1101 | P18 | state_licence | Netherlands | Netherlands physiotherapy board (synthetic) | active | 2027-11-28
CR-1201 | P21 | state_licence | Netherlands | Netherlands physiotherapy board (synthetic) | active | 2028-12-28
---page---
payer-contracts.csv — Payer contract and enrolment register

contract_id | payer | payer_class | effective_on | expires_on | auto_renews
BP-2023 | Insurer Bluepoint (synthetic) | commercial | 2023-01-01 | 2028-12-31 | yes
HG-2024 | Insurer Harrowgate (synthetic) | commercial | 2024-07-01 | 2029-06-30 | no
GS-ENR-118 | Government scheme (synthetic) | medicaid | 2019-04-01 |  | no
---page---
pnl.csv — Profit and loss by fiscal year, FY2023 to FY2025

Line | FY2023 | FY2024 | FY2025
Net patient service revenue | 2311930.40 | 2463532.78 | 2633909.34
Other operating revenue | 8280.00 | 8528.40 | 8776.80
Cost of care: clinical staff | 951286.26 | 1013545.08 | 1083501.32
Clinical and dental supplies | 157774.31 | 207653.14 | 272196.67
Laboratory fees | 71926.52 | 76633.90 | 79280.58
Rent and occupancy | 171695.57 | 180460.47 | 190273.40
General and administrative | 273784.83 | 254622.30 | 224628.32
