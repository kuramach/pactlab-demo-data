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
2021-01 | Insurer Bluepoint (synthetic) | commercial | 633 | 31 | 89999.10 | 68701.60 | 107537.08
2021-01 | Insurer Harrowgate (synthetic) | commercial | 367 | 18 | 51966.02 | 39668.72 | 61231.01
2021-01 | Government scheme (synthetic) | medicaid | 427 | 20 | 38366.05 | 29287.06 | 45160.88
2021-01 | Patients — self-pay (synthetic) | self_pay | 325 | 16 | 37490.77 | 28618.91 | 43731.01
2021-02 | Insurer Bluepoint (synthetic) | commercial | 636 | 30 | 90449.09 | 69045.11 | 106896.54
2021-02 | Insurer Harrowgate (synthetic) | commercial | 367 | 18 | 52225.85 | 39867.06 | 61599.02
2021-02 | Government scheme (synthetic) | medicaid | 434 | 20 | 38557.89 | 29433.50 | 45021.41
2021-02 | Patients — self-pay (synthetic) | self_pay | 327 | 16 | 37678.22 | 28762.00 | 43994.28
2021-03 | Insurer Bluepoint (synthetic) | commercial | 637 | 31 | 90901.33 | 69390.33 | 108938.07
2021-03 | Insurer Harrowgate (synthetic) | commercial | 365 | 17 | 52486.97 | 40066.39 | 61782.69
2021-03 | Government scheme (synthetic) | medicaid | 434 | 20 | 38750.68 | 29580.67 | 45934.85
2021-03 | Patients — self-pay (synthetic) | self_pay | 328 | 16 | 37866.61 | 28905.81 | 45200.77
2021-04 | Insurer Bluepoint (synthetic) | commercial | 637 | 30 | 91355.84 | 69737.28 | 106778.15
2021-04 | Insurer Harrowgate (synthetic) | commercial | 375 | 19 | 52749.42 | 40266.73 | 63278.48
2021-04 | Government scheme (synthetic) | medicaid | 436 | 21 | 38944.43 | 29728.57 | 46579.59
2021-04 | Patients — self-pay (synthetic) | self_pay | 327 | 16 | 38055.95 | 29050.34 | 44931.06
2021-05 | Insurer Bluepoint (synthetic) | commercial | 646 | 31 | 91812.62 | 70085.97 | 107094.59
2021-05 | Insurer Harrowgate (synthetic) | commercial | 374 | 17 | 53013.16 | 40468.06 | 62150.95
2021-05 | Government scheme (synthetic) | medicaid | 441 | 21 | 39139.15 | 29877.21 | 45746.46
2021-05 | Patients — self-pay (synthetic) | self_pay | 330 | 16 | 38246.22 | 29195.59 | 44974.54
2021-06 | Insurer Bluepoint (synthetic) | commercial | 649 | 32 | 92271.68 | 70436.40 | 107848.60
2021-06 | Insurer Harrowgate (synthetic) | commercial | 375 | 18 | 53278.22 | 40670.40 | 62209.33
2021-06 | Government scheme (synthetic) | medicaid | 444 | 21 | 39334.85 | 30026.60 | 47139.71
2021-06 | Patients — self-pay (synthetic) | self_pay | 334 | 16 | 38437.46 | 29341.57 | 45654.60
2021-07 | Insurer Bluepoint (synthetic) | commercial | 651 | 31 | 92733.04 | 70788.58 | 109925.26
2021-07 | Insurer Harrowgate (synthetic) | commercial | 380 | 18 | 53544.61 | 40873.75 | 63027.64
2021-07 | Government scheme (synthetic) | medicaid | 445 | 21 | 39531.52 | 30176.73 | 47515.85
2021-07 | Patients — self-pay (synthetic) | self_pay | 333 | 16 | 38629.65 | 29488.28 | 46386.08
2021-08 | Insurer Bluepoint (synthetic) | commercial | 655 | 32 | 93196.70 | 71142.52 | 110033.42
2021-08 | Insurer Harrowgate (synthetic) | commercial | 382 | 18 | 53812.34 | 41078.12 | 63980.04
2021-08 | Government scheme (synthetic) | medicaid | 448 | 22 | 39729.18 | 30327.62 | 46342.00
2021-08 | Patients — self-pay (synthetic) | self_pay | 337 | 16 | 38822.79 | 29635.72 | 46342.15
2021-09 | Insurer Bluepoint (synthetic) | commercial | 653 | 31 | 93662.69 | 71498.24 | 111027.26
2021-09 | Insurer Harrowgate (synthetic) | commercial | 378 | 18 | 54081.40 | 41283.51 | 63659.50
2021-09 | Government scheme (synthetic) | medicaid | 449 | 22 | 39927.82 | 30479.25 | 46951.96
2021-09 | Patients — self-pay (synthetic) | self_pay | 336 | 17 | 39016.91 | 29783.90 | 45880.81
2021-10 | Insurer Bluepoint (synthetic) | commercial | 663 | 32 | 94131.01 | 71855.73 | 111470.93
2021-10 | Insurer Harrowgate (synthetic) | commercial | 381 | 18 | 54351.81 | 41489.93 | 64299.62
2021-10 | Government scheme (synthetic) | medicaid | 454 | 22 | 40127.46 | 30631.65 | 47804.48
2021-10 | Patients — self-pay (synthetic) | self_pay | 338 | 17 | 39211.99 | 29932.82 | 45878.03
2021-11 | Insurer Bluepoint (synthetic) | commercial | 667 | 32 | 94601.66 | 72215.01 | 112476.39
2021-11 | Insurer Harrowgate (synthetic) | commercial | 383 | 19 | 54623.57 | 41697.38 | 65526.72
2021-11 | Government scheme (synthetic) | medicaid | 451 | 22 | 40328.10 | 30784.81 | 47995.75
2021-11 | Patients — self-pay (synthetic) | self_pay | 338 | 16 | 39408.05 | 30082.48 | 47087.43
2021-12 | Insurer Bluepoint (synthetic) | commercial | 675 | 33 | 95074.66 | 72576.08 | 112138.06
2021-12 | Insurer Harrowgate (synthetic) | commercial | 387 | 18 | 54896.69 | 41905.87 | 64814.21
2021-12 | Government scheme (synthetic) | medicaid | 452 | 21 | 40529.74 | 30938.73 | 47563.78
2021-12 | Patients — self-pay (synthetic) | self_pay | 340 | 16 | 39605.09 | 30232.89 | 46713.16
2022-01 | Insurer Bluepoint (synthetic) | commercial | 671 | 33 | 95550.04 | 72938.96 | 112925.06
2022-01 | Insurer Harrowgate (synthetic) | commercial | 389 | 19 | 55171.16 | 42115.39 | 64615.59
2022-01 | Government scheme (synthetic) | medicaid | 456 | 22 | 40732.39 | 31093.43 | 47994.55
2022-01 | Patients — self-pay (synthetic) | self_pay | 344 | 17 | 39803.12 | 30384.06 | 47559.49
2022-02 | Insurer Bluepoint (synthetic) | commercial | 675 | 33 | 96027.79 | 73303.66 | 115195.44
2022-02 | Insurer Harrowgate (synthetic) | commercial | 388 | 18 | 55447.02 | 42325.97 | 66645.86
2022-02 | Government scheme (synthetic) | medicaid | 462 | 22 | 40936.05 | 31248.89 | 48428.42
2022-02 | Patients — self-pay (synthetic) | self_pay | 347 | 17 | 40002.13 | 30535.98 | 47655.17
2022-03 | Insurer Bluepoint (synthetic) | commercial | 683 | 34 | 96507.92 | 73670.17 | 115771.41
2022-03 | Insurer Harrowgate (synthetic) | commercial | 394 | 19 | 55724.26 | 42537.60 | 66187.22
2022-03 | Government scheme (synthetic) | medicaid | 463 | 22 | 41140.73 | 31405.14 | 49109.04
2022-03 | Patients — self-pay (synthetic) | self_pay | 347 | 17 | 40202.14 | 30688.66 | 48274.31
… 216 more rows in remittances.csv
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
clinician-collections.csv — Collections by clinician and month, pseudonymous, from the practice-management system, January 2021 to September 2026

month | provider_ref | site | visits | collected
2021-01 | P01 | Site 1 (synthetic) | 302 | 32819.52
2021-01 | P02 | Site 1 (synthetic) | 140 | 15225.89
2021-01 | P03 | Site 1 (synthetic) | 107 | 11615.58
2021-01 | P04 | Site 2 (synthetic) | 115 | 12523.03
2021-01 | P05 | Site 2 (synthetic) | 124 | 13473.72
2021-01 | P06 | Site 4 (synthetic) | 138 | 14967.97
2021-01 | P09 | Site 3 (synthetic) | 115 | 12442.18
2021-01 | P13 | Site 4 (synthetic) | 98 | 10592.52
2021-01 | P14 | Site 5 (synthetic) | 97 | 10533.92
2021-01 | P17 | Site 5 (synthetic) | 94 | 10232.59
2021-01 | P18 | Site 6 (synthetic) | 100 | 10863.41
2021-01 | P21 | Site 6 (synthetic) | 101 | 10985.96
2021-02 | P01 | Site 1 (synthetic) | 304 | 32983.61
2021-02 | P02 | Site 1 (synthetic) | 141 | 15302.02
2021-02 | P03 | Site 1 (synthetic) | 108 | 11673.66
2021-02 | P04 | Site 2 (synthetic) | 116 | 12585.64
2021-02 | P05 | Site 2 (synthetic) | 125 | 13541.09
2021-02 | P06 | Site 4 (synthetic) | 139 | 15042.81
2021-02 | P09 | Site 3 (synthetic) | 115 | 12504.39
2021-02 | P13 | Site 4 (synthetic) | 98 | 10645.48
2021-02 | P14 | Site 5 (synthetic) | 98 | 10586.59
2021-02 | P17 | Site 5 (synthetic) | 95 | 10283.76
2021-02 | P18 | Site 6 (synthetic) | 101 | 10917.73
2021-02 | P21 | Site 6 (synthetic) | 102 | 11040.89
2021-03 | P01 | Site 1 (synthetic) | 305 | 33148.53
2021-03 | P02 | Site 1 (synthetic) | 142 | 15378.53
2021-03 | P03 | Site 1 (synthetic) | 108 | 11732.03
2021-03 | P04 | Site 2 (synthetic) | 117 | 12648.57
2021-03 | P05 | Site 2 (synthetic) | 125 | 13608.79
2021-03 | P06 | Site 4 (synthetic) | 139 | 15118.02
2021-03 | P09 | Site 3 (synthetic) | 116 | 12566.91
2021-03 | P13 | Site 4 (synthetic) | 99 | 10698.71
2021-03 | P14 | Site 5 (synthetic) | 98 | 10639.53
2021-03 | P17 | Site 5 (synthetic) | 95 | 10335.18
2021-03 | P18 | Site 6 (synthetic) | 101 | 10972.31
2021-03 | P21 | Site 6 (synthetic) | 102 | 11096.09
2021-04 | P01 | Site 1 (synthetic) | 307 | 33314.27
2021-04 | P02 | Site 1 (synthetic) | 142 | 15455.42
2021-04 | P03 | Site 1 (synthetic) | 109 | 11790.69
2021-04 | P04 | Site 2 (synthetic) | 117 | 12711.81
2021-04 | P05 | Site 2 (synthetic) | 126 | 13676.84
2021-04 | P06 | Site 4 (synthetic) | 140 | 15193.61
2021-04 | P09 | Site 3 (synthetic) | 116 | 12629.74
2021-04 | P13 | Site 4 (synthetic) | 99 | 10752.20
2021-04 | P14 | Site 5 (synthetic) | 98 | 10692.72
2021-04 | P17 | Site 5 (synthetic) | 96 | 10386.85
2021-04 | P18 | Site 6 (synthetic) | 102 | 11027.18
2021-04 | P21 | Site 6 (synthetic) | 103 | 11151.59
2021-05 | P01 | Site 1 (synthetic) | 308 | 33480.84
2021-05 | P02 | Site 1 (synthetic) | 143 | 15532.70
2021-05 | P03 | Site 1 (synthetic) | 109 | 11849.64
2021-05 | P04 | Site 2 (synthetic) | 118 | 12775.37
2021-05 | P05 | Site 2 (synthetic) | 127 | 13745.22
2021-05 | P06 | Site 4 (synthetic) | 141 | 15269.58
2021-05 | P09 | Site 3 (synthetic) | 117 | 12692.89
2021-05 | P13 | Site 4 (synthetic) | 100 | 10805.96
2021-05 | P14 | Site 5 (synthetic) | 99 | 10746.19
2021-05 | P17 | Site 5 (synthetic) | 96 | 10438.79
2021-05 | P18 | Site 6 (synthetic) | 102 | 11082.31
2021-05 | P21 | Site 6 (synthetic) | 103 | 11207.34
… 768 more rows in clinician-collections.csv
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
pnl.csv — Profit and loss by fiscal year, FY2021 to FY2025

Line | FY2021 | FY2022 | FY2023 | FY2024 | FY2025
Net patient service revenue | 2051111.48 | 2177619.54 | 2311930.40 | 2463532.78 | 2633909.34
Other operating revenue | 7783.20 | 8031.60 | 8280.00 | 8528.40 | 8776.80
Cost of care: clinical staff | 844146.82 | 896116.97 | 951286.26 | 1013545.08 | 1083501.32
Clinical and dental supplies | 92650.26 | 122396.46 | 157774.31 | 207653.14 | 272196.67
Laboratory fees | 63825.74 | 67755.19 | 71926.52 | 76633.90 | 79280.58
Rent and occupancy | 156476.00 | 163923.84 | 171695.57 | 180460.47 | 190273.40
General and administrative | 308834.20 | 290691.60 | 273784.83 | 254622.30 | 224628.32
