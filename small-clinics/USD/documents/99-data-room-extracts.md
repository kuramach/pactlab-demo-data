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
2021-01 | Insurer Bluepoint (synthetic) | commercial | 664 | 32 | 101864.30 | 77759.01 | 119784.37
2021-01 | Insurer Harrowgate (synthetic) | commercial | 379 | 18 | 57976.89 | 44257.17 | 67832.96
2021-01 | Government scheme (synthetic) | medicaid | 439 | 21 | 42745.00 | 32629.77 | 50619.08
2021-01 | Patients — self-pay (synthetic) | self_pay | 320 | 15 | 39832.08 | 30406.17 | 46839.38
2021-02 | Insurer Bluepoint (synthetic) | commercial | 662 | 31 | 102373.63 | 78147.81 | 122323.02
2021-02 | Insurer Harrowgate (synthetic) | commercial | 374 | 18 | 58266.78 | 44478.46 | 69483.14
2021-02 | Government scheme (synthetic) | medicaid | 445 | 21 | 42958.73 | 32792.92 | 50261.71
2021-02 | Patients — self-pay (synthetic) | self_pay | 320 | 15 | 40031.24 | 30558.20 | 46789.15
2021-03 | Insurer Bluepoint (synthetic) | commercial | 664 | 32 | 102885.50 | 78538.55 | 120619.71
2021-03 | Insurer Harrowgate (synthetic) | commercial | 377 | 18 | 58558.11 | 44700.85 | 69691.86
2021-03 | Government scheme (synthetic) | medicaid | 445 | 22 | 43173.51 | 32956.88 | 50615.26
2021-03 | Patients — self-pay (synthetic) | self_pay | 322 | 15 | 40231.41 | 30711.00 | 46975.46
2021-04 | Insurer Bluepoint (synthetic) | commercial | 676 | 32 | 103399.92 | 78931.24 | 121590.14
2021-04 | Insurer Harrowgate (synthetic) | commercial | 377 | 18 | 58850.91 | 44924.36 | 68785.87
2021-04 | Government scheme (synthetic) | medicaid | 444 | 21 | 43389.39 | 33121.67 | 51022.50
2021-04 | Patients — self-pay (synthetic) | self_pay | 318 | 15 | 40432.56 | 30864.55 | 48263.71
2021-05 | Insurer Bluepoint (synthetic) | commercial | 666 | 32 | 103916.93 | 79325.90 | 121582.81
2021-05 | Insurer Harrowgate (synthetic) | commercial | 380 | 18 | 59145.16 | 45148.98 | 70600.64
2021-05 | Government scheme (synthetic) | medicaid | 454 | 22 | 43606.34 | 33287.28 | 50916.14
2021-05 | Patients — self-pay (synthetic) | self_pay | 325 | 16 | 40634.72 | 31018.87 | 47638.86
2021-06 | Insurer Bluepoint (synthetic) | commercial | 672 | 33 | 104436.51 | 79722.53 | 122067.04
2021-06 | Insurer Harrowgate (synthetic) | commercial | 384 | 19 | 59440.88 | 45374.72 | 70249.73
2021-06 | Government scheme (synthetic) | medicaid | 451 | 22 | 43824.36 | 33453.71 | 52156.75
2021-06 | Patients — self-pay (synthetic) | self_pay | 327 | 15 | 40837.90 | 31173.97 | 48167.23
2021-07 | Insurer Bluepoint (synthetic) | commercial | 673 | 31 | 104958.69 | 80121.14 | 125660.41
2021-07 | Insurer Harrowgate (synthetic) | commercial | 386 | 19 | 59738.10 | 45601.60 | 70813.23
2021-07 | Government scheme (synthetic) | medicaid | 451 | 22 | 44043.48 | 33620.98 | 52626.16
2021-07 | Patients — self-pay (synthetic) | self_pay | 323 | 15 | 41042.09 | 31329.84 | 48748.28
2021-08 | Insurer Bluepoint (synthetic) | commercial | 687 | 33 | 105483.48 | 80521.74 | 124539.90
2021-08 | Insurer Harrowgate (synthetic) | commercial | 388 | 19 | 60036.78 | 45829.60 | 70171.94
2021-08 | Government scheme (synthetic) | medicaid | 458 | 22 | 44263.71 | 33789.09 | 51631.29
2021-08 | Patients — self-pay (synthetic) | self_pay | 325 | 16 | 41247.30 | 31486.49 | 48112.80
2021-09 | Insurer Bluepoint (synthetic) | commercial | 690 | 33 | 106010.90 | 80924.35 | 126669.08
2021-09 | Insurer Harrowgate (synthetic) | commercial | 388 | 19 | 60336.96 | 46058.75 | 70379.89
2021-09 | Government scheme (synthetic) | medicaid | 460 | 22 | 44485.02 | 33958.03 | 52047.47
2021-09 | Patients — self-pay (synthetic) | self_pay | 328 | 15 | 41453.54 | 31643.92 | 48942.45
2021-10 | Insurer Bluepoint (synthetic) | commercial | 691 | 33 | 106540.95 | 81328.97 | 127554.75
2021-10 | Insurer Harrowgate (synthetic) | commercial | 391 | 18 | 60638.66 | 46289.05 | 71090.85
2021-10 | Government scheme (synthetic) | medicaid | 463 | 23 | 44707.44 | 34127.82 | 53048.91
2021-10 | Patients — self-pay (synthetic) | self_pay | 329 | 16 | 41660.80 | 31802.14 | 49976.51
2021-11 | Insurer Bluepoint (synthetic) | commercial | 695 | 34 | 107073.66 | 81735.62 | 125910.17
2021-11 | Insurer Harrowgate (synthetic) | commercial | 398 | 19 | 60941.84 | 46520.49 | 72384.47
2021-11 | Government scheme (synthetic) | medicaid | 467 | 22 | 44930.98 | 34298.46 | 53101.32
2021-11 | Patients — self-pay (synthetic) | self_pay | 330 | 16 | 41869.11 | 31961.15 | 49433.10
2021-12 | Insurer Bluepoint (synthetic) | commercial | 693 | 33 | 107609.03 | 82144.30 | 127304.31
2021-12 | Insurer Harrowgate (synthetic) | commercial | 393 | 19 | 61246.55 | 46753.09 | 72456.28
2021-12 | Government scheme (synthetic) | medicaid | 465 | 22 | 45155.63 | 34469.95 | 53420.30
2021-12 | Patients — self-pay (synthetic) | self_pay | 335 | 16 | 42078.46 | 32120.96 | 49779.93
2022-01 | Insurer Bluepoint (synthetic) | commercial | 704 | 34 | 108147.08 | 82555.02 | 126404.01
2022-01 | Insurer Harrowgate (synthetic) | commercial | 398 | 19 | 61552.79 | 46986.86 | 73110.14
2022-01 | Government scheme (synthetic) | medicaid | 472 | 23 | 45381.41 | 34642.30 | 54117.33
2022-01 | Patients — self-pay (synthetic) | self_pay | 339 | 16 | 42288.84 | 32281.56 | 50830.07
2022-02 | Insurer Bluepoint (synthetic) | commercial | 708 | 34 | 108687.80 | 82967.79 | 130639.88
2022-02 | Insurer Harrowgate (synthetic) | commercial | 397 | 20 | 61860.54 | 47221.79 | 73109.39
2022-02 | Government scheme (synthetic) | medicaid | 468 | 22 | 45608.32 | 34815.51 | 53469.75
2022-02 | Patients — self-pay (synthetic) | self_pay | 339 | 16 | 42500.29 | 32442.97 | 49876.33
2022-03 | Insurer Bluepoint (synthetic) | commercial | 714 | 33 | 109231.25 | 83382.63 | 130775.68
2022-03 | Insurer Harrowgate (synthetic) | commercial | 400 | 19 | 62169.85 | 47457.90 | 73990.30
2022-03 | Government scheme (synthetic) | medicaid | 473 | 23 | 45836.36 | 34989.59 | 54876.98
2022-03 | Patients — self-pay (synthetic) | self_pay | 337 | 16 | 42712.79 | 32605.18 | 49973.96
… 216 more rows in remittances.csv
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
clinician-collections.csv — Collections by clinician and month, pseudonymous, from the practice-management system, January 2021 to September 2026

month | provider_ref | site | visits | collected
2021-01 | P01 | Site 1 (synthetic) | 308 | 36309.51
2021-01 | P02 | Site 1 (synthetic) | 135 | 15936.04
2021-01 | P03 | Site 1 (synthetic) | 115 | 13586.60
2021-01 | P04 | Site 2 (synthetic) | 119 | 13986.35
2021-01 | P05 | Site 2 (synthetic) | 137 | 16215.54
2021-01 | P06 | Site 4 (synthetic) | 141 | 16662.89
2021-01 | P09 | Site 3 (synthetic) | 111 | 13138.52
2021-01 | P13 | Site 4 (synthetic) | 98 | 11530.34
2021-01 | P14 | Site 5 (synthetic) | 105 | 12389.56
2021-01 | P17 | Site 5 (synthetic) | 100 | 11835.06
2021-01 | P18 | Site 6 (synthetic) | 98 | 11607.54
2021-01 | P21 | Site 6 (synthetic) | 100 | 11854.17
2021-02 | P01 | Site 1 (synthetic) | 309 | 36491.05
2021-02 | P02 | Site 1 (synthetic) | 136 | 16015.72
2021-02 | P03 | Site 1 (synthetic) | 116 | 13654.53
2021-02 | P04 | Site 2 (synthetic) | 119 | 14056.28
2021-02 | P05 | Site 2 (synthetic) | 138 | 16296.62
2021-02 | P06 | Site 4 (synthetic) | 142 | 16746.21
2021-02 | P09 | Site 3 (synthetic) | 112 | 13204.22
2021-02 | P13 | Site 4 (synthetic) | 98 | 11587.99
2021-02 | P14 | Site 5 (synthetic) | 106 | 12451.51
2021-02 | P17 | Site 5 (synthetic) | 101 | 11894.24
2021-02 | P18 | Site 6 (synthetic) | 99 | 11665.58
2021-02 | P21 | Site 6 (synthetic) | 101 | 11913.44
2021-03 | P01 | Site 1 (synthetic) | 311 | 36673.51
2021-03 | P02 | Site 1 (synthetic) | 136 | 16095.80
2021-03 | P03 | Site 1 (synthetic) | 116 | 13722.80
2021-03 | P04 | Site 2 (synthetic) | 120 | 14126.56
2021-03 | P05 | Site 2 (synthetic) | 139 | 16378.10
2021-03 | P06 | Site 4 (synthetic) | 143 | 16829.94
2021-03 | P09 | Site 3 (synthetic) | 112 | 13270.24
2021-03 | P13 | Site 4 (synthetic) | 99 | 11645.93
2021-03 | P14 | Site 5 (synthetic) | 106 | 12513.77
2021-03 | P17 | Site 5 (synthetic) | 101 | 11953.71
2021-03 | P18 | Site 6 (synthetic) | 99 | 11723.91
2021-03 | P21 | Site 6 (synthetic) | 101 | 11973.01
2021-04 | P01 | Site 1 (synthetic) | 312 | 36856.88
2021-04 | P02 | Site 1 (synthetic) | 137 | 16176.28
2021-04 | P03 | Site 1 (synthetic) | 117 | 13791.42
2021-04 | P04 | Site 2 (synthetic) | 120 | 14197.19
2021-04 | P05 | Site 2 (synthetic) | 139 | 16459.99
2021-04 | P06 | Site 4 (synthetic) | 143 | 16914.09
2021-04 | P09 | Site 3 (synthetic) | 113 | 13336.59
2021-04 | P13 | Site 4 (synthetic) | 99 | 11704.16
2021-04 | P14 | Site 5 (synthetic) | 107 | 12576.34
2021-04 | P17 | Site 5 (synthetic) | 102 | 12013.48
2021-04 | P18 | Site 6 (synthetic) | 100 | 11782.53
2021-04 | P21 | Site 6 (synthetic) | 102 | 12032.87
2021-05 | P01 | Site 1 (synthetic) | 314 | 37041.16
2021-05 | P02 | Site 1 (synthetic) | 138 | 16257.16
2021-05 | P03 | Site 1 (synthetic) | 117 | 13860.37
2021-05 | P04 | Site 2 (synthetic) | 121 | 14268.18
2021-05 | P05 | Site 2 (synthetic) | 140 | 16542.29
2021-05 | P06 | Site 4 (synthetic) | 144 | 16998.66
2021-05 | P09 | Site 3 (synthetic) | 114 | 13403.27
2021-05 | P13 | Site 4 (synthetic) | 100 | 11762.68
2021-05 | P14 | Site 5 (synthetic) | 107 | 12639.22
2021-05 | P17 | Site 5 (synthetic) | 102 | 12073.54
2021-05 | P18 | Site 6 (synthetic) | 100 | 11841.44
2021-05 | P21 | Site 6 (synthetic) | 102 | 12093.06
… 768 more rows in clinician-collections.csv
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
pnl.csv — Profit and loss by fiscal year, FY2021 to FY2025

Line | FY2021 | FY2022 | FY2023 | FY2024 | FY2025
Net patient service revenue | 2282722.10 | 2423515.37 | 2572992.55 | 2722434.86 | 2867350.10
Other operating revenue | 8460.00 | 8730.00 | 9000.00 | 9270.00 | 9540.00
Cost of care: clinical staff | 939384.66 | 997220.60 | 1058616.95 | 1119998.99 | 1179524.94
Clinical and dental supplies | 103103.19 | 136205.74 | 175575.49 | 229463.21 | 296319.68
Laboratory fees | 71026.65 | 75399.61 | 80041.77 | 84682.85 | 86306.70
Rent and occupancy | 174129.84 | 182418.40 | 191067.45 | 199414.45 | 207136.09
General and administrative | 343677.32 | 323488.63 | 304675.12 | 281365.60 | 244535.66
