Clearbrook Clinics Ltd — data-room extracts (synthetic demo data)

Each page reproduces one structured extract from this folder. All names and figures are fictional.
---page---
patient-volume.csv — Visits and revenue by site and pseudonymous provider

month | site | provider_ref | visits | revenue
2025-10 | Site 1 | P01 | 200 | 16590.00
2025-10 | Site 1 | P02 | 174 | 14433.30
2025-10 | Site 1 | P03 | 168 | 13935.60
2025-10 | Site 1 | P04 | 197 | 16341.15
2025-10 | Site 2 | P05 | 132 | 10949.40
2025-10 | Site 2 | P06 | 141 | 11695.95
2025-10 | Site 2 | P07 | 156 | 12940.20
2025-10 | Site 2 | P08 | 181 | 15013.95
2025-10 | Site 3 | P07 | 240 | 19908.00
2025-10 | Site 3 | P08 | 85 | 7050.75
2025-10 | Site 4 | P13 | 139 | 11530.05
2025-10 | Site 4 | P14 | 132 | 10949.40
2025-10 | Site 4 | P15 | 139 | 11530.05
2025-10 | Site 4 | P16 | 154 | 12774.30
2025-10 | Site 5 | P17 | 135 | 11198.25
2025-10 | Site 5 | P18 | 142 | 11778.90
2025-10 | Site 5 | P19 | 182 | 15096.90
2025-10 | Site 5 | P20 | 144 | 11944.80
2025-10 | Site 6 | P21 | 191 | 15843.45
2025-10 | Site 6 | P22 | 184 | 15262.80
2025-10 | Site 6 | P23 | 166 | 13769.70
2025-10 | Site 6 | P24 | 151 | 12525.45
2025-11 | Site 1 | P01 | 165 | 13686.75
2025-11 | Site 1 | P02 | 173 | 14350.35
2025-11 | Site 1 | P03 | 121 | 10036.95
2025-11 | Site 1 | P04 | 191 | 15843.45
2025-11 | Site 2 | P05 | 129 | 10700.55
2025-11 | Site 2 | P06 | 162 | 13437.90
2025-11 | Site 2 | P07 | 149 | 12359.55
2025-11 | Site 2 | P08 | 189 | 15677.55
2025-11 | Site 3 | P07 | 240 | 19908.00
2025-11 | Site 3 | P08 | 85 | 7050.75
2025-11 | Site 4 | P13 | 184 | 15262.80
2025-11 | Site 4 | P14 | 155 | 12857.25
2025-11 | Site 4 | P15 | 178 | 14765.10
2025-11 | Site 4 | P16 | 186 | 15428.70
2025-11 | Site 5 | P17 | 199 | 16507.05
2025-11 | Site 5 | P18 | 135 | 11198.25
2025-11 | Site 5 | P19 | 120 | 9954.00
2025-11 | Site 5 | P20 | 138 | 11447.10
2025-11 | Site 6 | P21 | 187 | 15511.65
2025-11 | Site 6 | P22 | 185 | 15345.75
2025-11 | Site 6 | P23 | 169 | 14018.55
2025-11 | Site 6 | P24 | 195 | 16175.25
2025-12 | Site 1 | P01 | 125 | 10368.75
2025-12 | Site 1 | P02 | 188 | 15594.60
2025-12 | Site 1 | P03 | 165 | 13686.75
2025-12 | Site 1 | P04 | 199 | 16507.05
2025-12 | Site 2 | P05 | 163 | 13520.85
2025-12 | Site 2 | P06 | 175 | 14516.25
2025-12 | Site 2 | P07 | 122 | 10119.90
2025-12 | Site 2 | P08 | 148 | 12276.60
2025-12 | Site 3 | P07 | 240 | 19908.00
2025-12 | Site 3 | P08 | 85 | 7050.75
2025-12 | Site 4 | P13 | 180 | 14931.00
2025-12 | Site 4 | P14 | 129 | 10700.55
2025-12 | Site 4 | P15 | 193 | 16009.35
2025-12 | Site 4 | P16 | 122 | 10119.90
2025-12 | Site 5 | P17 | 132 | 10949.40
2025-12 | Site 5 | P18 | 129 | 10700.55
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
2021-01 | Insurer Bluepoint (synthetic) | commercial | 627 | 29 | 77067.52 | 58830.17 | 91264.17
2021-01 | Insurer Harrowgate (synthetic) | commercial | 375 | 18 | 45895.51 | 35034.74 | 53752.10
2021-01 | Government scheme (synthetic) | medicaid | 432 | 20 | 33087.14 | 25257.36 | 38829.50
2021-01 | Patients — self-pay (synthetic) | self_pay | 326 | 15 | 32268.56 | 24632.49 | 37677.79
2021-02 | Insurer Bluepoint (synthetic) | commercial | 641 | 30 | 77452.86 | 59124.32 | 90344.68
2021-02 | Insurer Harrowgate (synthetic) | commercial | 380 | 18 | 46124.98 | 35209.91 | 55113.28
2021-02 | Government scheme (synthetic) | medicaid | 430 | 21 | 33252.58 | 25383.65 | 39889.97
2021-02 | Patients — self-pay (synthetic) | self_pay | 327 | 16 | 32429.90 | 24755.65 | 38711.06
2021-03 | Insurer Bluepoint (synthetic) | commercial | 638 | 30 | 77840.12 | 59419.94 | 91902.55
2021-03 | Insurer Harrowgate (synthetic) | commercial | 380 | 18 | 46355.61 | 35385.96 | 55498.64
2021-03 | Government scheme (synthetic) | medicaid | 434 | 21 | 33418.85 | 25510.57 | 39020.90
2021-03 | Patients — self-pay (synthetic) | self_pay | 329 | 15 | 32592.05 | 24879.43 | 39097.59
2021-04 | Insurer Bluepoint (synthetic) | commercial | 635 | 31 | 78229.32 | 59717.04 | 93010.54
2021-04 | Insurer Harrowgate (synthetic) | commercial | 380 | 19 | 46587.39 | 35562.89 | 55941.65
2021-04 | Government scheme (synthetic) | medicaid | 438 | 22 | 33585.94 | 25638.12 | 39852.37
2021-04 | Patients — self-pay (synthetic) | self_pay | 332 | 16 | 32755.02 | 25003.83 | 38905.21
2021-05 | Insurer Bluepoint (synthetic) | commercial | 650 | 31 | 78620.46 | 60015.62 | 92358.35
2021-05 | Insurer Harrowgate (synthetic) | commercial | 387 | 18 | 46820.33 | 35740.71 | 55278.79
2021-05 | Government scheme (synthetic) | medicaid | 439 | 21 | 33753.87 | 25766.31 | 39811.80
2021-05 | Patients — self-pay (synthetic) | self_pay | 330 | 16 | 32918.79 | 25128.85 | 38865.83
2021-06 | Insurer Bluepoint (synthetic) | commercial | 649 | 31 | 79013.57 | 60315.70 | 94691.53
2021-06 | Insurer Harrowgate (synthetic) | commercial | 388 | 19 | 47054.43 | 35919.41 | 55388.02
2021-06 | Government scheme (synthetic) | medicaid | 441 | 21 | 33922.63 | 25895.14 | 39850.16
2021-06 | Patients — self-pay (synthetic) | self_pay | 336 | 16 | 33083.38 | 25254.49 | 39177.69
2021-07 | Insurer Bluepoint (synthetic) | commercial | 645 | 31 | 79408.64 | 60617.28 | 95070.95
2021-07 | Insurer Harrowgate (synthetic) | commercial | 385 | 19 | 47289.70 | 36099.01 | 56560.97
2021-07 | Government scheme (synthetic) | medicaid | 448 | 22 | 34092.25 | 26024.62 | 40089.79
2021-07 | Patients — self-pay (synthetic) | self_pay | 332 | 16 | 33248.81 | 25380.77 | 39176.72
2021-08 | Insurer Bluepoint (synthetic) | commercial | 652 | 31 | 79805.68 | 60920.37 | 93183.63
2021-08 | Insurer Harrowgate (synthetic) | commercial | 391 | 19 | 47526.15 | 36279.50 | 56674.93
2021-08 | Government scheme (synthetic) | medicaid | 445 | 21 | 34262.71 | 26154.74 | 41142.30
2021-08 | Patients — self-pay (synthetic) | self_pay | 337 | 16 | 33415.05 | 25507.67 | 38976.90
2021-09 | Insurer Bluepoint (synthetic) | commercial | 650 | 31 | 80204.71 | 61224.97 | 93934.49
2021-09 | Insurer Harrowgate (synthetic) | commercial | 388 | 19 | 47763.78 | 36460.90 | 56166.43
2021-09 | Government scheme (synthetic) | medicaid | 453 | 21 | 34434.02 | 26285.51 | 40858.68
2021-09 | Patients — self-pay (synthetic) | self_pay | 339 | 16 | 33582.13 | 25635.21 | 39688.78
2021-10 | Insurer Bluepoint (synthetic) | commercial | 655 | 32 | 80605.73 | 61531.09 | 96695.06
2021-10 | Insurer Harrowgate (synthetic) | commercial | 390 | 18 | 48002.61 | 36643.21 | 56958.89
2021-10 | Government scheme (synthetic) | medicaid | 456 | 22 | 34606.19 | 26416.94 | 40571.20
2021-10 | Patients — self-pay (synthetic) | self_pay | 340 | 16 | 33750.03 | 25763.38 | 39887.21
2021-11 | Insurer Bluepoint (synthetic) | commercial | 661 | 32 | 81008.76 | 61838.75 | 94876.18
2021-11 | Insurer Harrowgate (synthetic) | commercial | 393 | 19 | 48242.61 | 36826.42 | 57643.57
2021-11 | Government scheme (synthetic) | medicaid | 451 | 21 | 34779.23 | 26549.03 | 41062.37
2021-11 | Patients — self-pay (synthetic) | self_pay | 342 | 17 | 33918.78 | 25892.20 | 40488.31
2021-12 | Insurer Bluepoint (synthetic) | commercial | 669 | 32 | 81413.80 | 62147.94 | 96121.85
2021-12 | Insurer Harrowgate (synthetic) | commercial | 393 | 19 | 48483.82 | 37010.55 | 57644.71
2021-12 | Government scheme (synthetic) | medicaid | 454 | 22 | 34953.12 | 26681.77 | 41681.60
2021-12 | Patients — self-pay (synthetic) | self_pay | 344 | 17 | 34088.37 | 26021.66 | 40932.96
2022-01 | Insurer Bluepoint (synthetic) | commercial | 665 | 33 | 81820.87 | 62458.68 | 97086.92
2022-01 | Insurer Harrowgate (synthetic) | commercial | 396 | 18 | 48726.25 | 37195.61 | 57298.22
2022-01 | Government scheme (synthetic) | medicaid | 459 | 22 | 35127.89 | 26815.18 | 41890.01
2022-01 | Patients — self-pay (synthetic) | self_pay | 344 | 16 | 34258.82 | 26151.77 | 40407.38
2022-02 | Insurer Bluepoint (synthetic) | commercial | 673 | 32 | 82229.97 | 62770.97 | 96014.31
2022-02 | Insurer Harrowgate (synthetic) | commercial | 399 | 20 | 48969.87 | 37381.58 | 58280.59
2022-02 | Government scheme (synthetic) | medicaid | 466 | 23 | 35303.53 | 26949.26 | 41346.94
2022-02 | Patients — self-pay (synthetic) | self_pay | 348 | 17 | 34430.11 | 26282.53 | 40731.73
2022-03 | Insurer Bluepoint (synthetic) | commercial | 672 | 32 | 82641.13 | 63084.83 | 97962.36
2022-03 | Insurer Harrowgate (synthetic) | commercial | 402 | 19 | 49214.72 | 37568.49 | 59038.24
2022-03 | Government scheme (synthetic) | medicaid | 459 | 23 | 35480.04 | 27084.00 | 42183.90
2022-03 | Patients — self-pay (synthetic) | self_pay | 346 | 17 | 34602.26 | 26413.94 | 40730.50
… 216 more rows in remittances.csv
---page---
service-lines.csv — Collections and direct costs by month, service line and pseudonymous provider, from the schedule and billing exports

month | service_line | provider_ref | visits | collected | direct_cost
2025-10 | Implants | P01 | 133 | 32660.14 | 11104.45
2025-10 | Restorative dentistry | P01 | 55 | 5223.22 | 2402.68
2025-10 | Restorative dentistry | P02 | 165 | 15669.66 | 7208.04
2025-10 | Restorative dentistry | P05 | 165 | 15669.66 | 7208.04
2025-10 | Restorative dentistry | P06 | 202 | 19151.81 | 8809.83
2025-10 | Hygiene | P03 | 247 | 16604.52 | 8634.35
2025-10 | Hygiene | P04 | 202 | 13585.52 | 7064.47
2025-10 | Hygiene | P09 | 180 | 12076.02 | 6279.53
2025-10 | Physiotherapy | P13 | 144 | 9643.59 | 5303.97
2025-10 | Physiotherapy | P14 | 215 | 14465.39 | 7955.96
2025-10 | Physiotherapy | P17 | 197 | 13259.94 | 7292.97
2025-10 | Physiotherapy | P18 | 215 | 14465.39 | 7955.96
2025-10 | Physiotherapy | P21 | 144 | 9643.60 | 5303.98
2025-11 | Implants | P01 | 134 | 32804.40 | 11153.50
2025-11 | Restorative dentistry | P01 | 51 | 4796.61 | 2206.44
2025-11 | Restorative dentistry | P02 | 169 | 15988.70 | 7354.80
2025-11 | Restorative dentistry | P05 | 186 | 17587.57 | 8090.28
2025-11 | Restorative dentistry | P06 | 186 | 17587.56 | 8090.28
2025-11 | Hygiene | P03 | 217 | 14555.23 | 7568.72
2025-11 | Hygiene | P04 | 199 | 13342.29 | 6937.99
2025-11 | Hygiene | P09 | 217 | 14555.23 | 7568.72
2025-11 | Physiotherapy | P13 | 177 | 11874.89 | 6531.19
2025-11 | Physiotherapy | P14 | 212 | 14249.87 | 7837.43
2025-11 | Physiotherapy | P17 | 159 | 10687.40 | 5878.07
2025-11 | Physiotherapy | P18 | 212 | 14249.87 | 7837.43
2025-11 | Physiotherapy | P21 | 159 | 10687.41 | 5878.08
2025-12 | Implants | P01 | 136 | 33407.32 | 11358.49
2025-12 | Restorative dentistry | P01 | 56 | 5342.72 | 2457.65
2025-12 | Restorative dentistry | P02 | 150 | 14247.24 | 6553.73
2025-12 | Restorative dentistry | P05 | 188 | 17809.05 | 8192.16
2025-12 | Restorative dentistry | P06 | 207 | 19589.95 | 9011.38
2025-12 | Hygiene | P03 | 228 | 15340.75 | 7977.19
2025-12 | Hygiene | P04 | 166 | 11156.91 | 5801.59
2025-12 | Hygiene | P09 | 249 | 16735.35 | 8702.38
2025-12 | Physiotherapy | P13 | 174 | 11699.42 | 6434.68
2025-12 | Physiotherapy | P14 | 174 | 11699.42 | 6434.68
2025-12 | Physiotherapy | P17 | 174 | 11699.42 | 6434.68
2025-12 | Physiotherapy | P18 | 196 | 13161.85 | 7239.02
2025-12 | Physiotherapy | P21 | 218 | 14624.27 | 8043.35
2026-01 | Implants | P01 | 137 | 33615.65 | 11429.32
2026-01 | Restorative dentistry | P01 | 53 | 5059.80 | 2327.51
2026-01 | Restorative dentistry | P02 | 213 | 20239.18 | 9310.02
2026-01 | Restorative dentistry | P05 | 142 | 13492.79 | 6206.68
2026-01 | Restorative dentistry | P06 | 196 | 18552.58 | 8534.19
2026-01 | Hygiene | P03 | 251 | 16839.72 | 8756.65
2026-01 | Hygiene | P04 | 188 | 12629.79 | 6567.49
2026-01 | Hygiene | P09 | 209 | 14033.10 | 7297.21
2026-01 | Physiotherapy | P13 | 217 | 14602.27 | 8031.25
2026-01 | Physiotherapy | P14 | 163 | 10951.71 | 6023.44
2026-01 | Physiotherapy | P17 | 217 | 14602.27 | 8031.25
2026-01 | Physiotherapy | P18 | 199 | 13385.42 | 7361.98
2026-01 | Physiotherapy | P21 | 145 | 9734.85 | 5354.17
2026-02 | Implants | P01 | 137 | 33628.30 | 11433.62
2026-02 | Restorative dentistry | P01 | 50 | 4780.49 | 2199.03
2026-02 | Restorative dentistry | P02 | 151 | 14341.48 | 6597.08
2026-02 | Restorative dentistry | P05 | 202 | 19121.97 | 8796.11
2026-02 | Restorative dentistry | P06 | 202 | 19121.98 | 8796.11
2026-02 | Hygiene | P03 | 210 | 14079.67 | 7321.43
2026-02 | Hygiene | P04 | 229 | 15359.64 | 7987.01
2026-02 | Hygiene | P09 | 210 | 14079.66 | 7321.42
… 96 more rows in service-lines.csv
---page---
clinician-collections.csv — Collections by clinician and month, pseudonymous, from the practice-management system, January 2021 to September 2026

month | provider_ref | site | visits | collected
2021-01 | P01 | Site 1 (synthetic) | 303 | 28248.13
2021-01 | P02 | Site 1 (synthetic) | 128 | 11927.39
2021-01 | P03 | Site 1 (synthetic) | 116 | 10859.68
2021-01 | P04 | Site 2 (synthetic) | 109 | 10132.75
2021-01 | P05 | Site 2 (synthetic) | 136 | 12664.22
2021-01 | P06 | Site 4 (synthetic) | 143 | 13287.46
2021-01 | P09 | Site 3 (synthetic) | 114 | 10633.62
2021-01 | P13 | Site 4 (synthetic) | 95 | 8890.85
2021-01 | P14 | Site 5 (synthetic) | 103 | 9580.19
2021-01 | P17 | Site 5 (synthetic) | 99 | 9191.35
2021-01 | P18 | Site 6 (synthetic) | 100 | 9331.51
2021-01 | P21 | Site 6 (synthetic) | 97 | 9007.61
2021-02 | P01 | Site 1 (synthetic) | 305 | 28389.37
2021-02 | P02 | Site 1 (synthetic) | 129 | 11987.02
2021-02 | P03 | Site 1 (synthetic) | 117 | 10913.98
2021-02 | P04 | Site 2 (synthetic) | 109 | 10183.41
2021-02 | P05 | Site 2 (synthetic) | 137 | 12727.54
2021-02 | P06 | Site 4 (synthetic) | 143 | 13353.89
2021-02 | P09 | Site 3 (synthetic) | 115 | 10686.79
2021-02 | P13 | Site 4 (synthetic) | 96 | 8935.30
2021-02 | P14 | Site 5 (synthetic) | 103 | 9628.09
2021-02 | P17 | Site 5 (synthetic) | 99 | 9237.31
2021-02 | P18 | Site 6 (synthetic) | 101 | 9378.16
2021-02 | P21 | Site 6 (synthetic) | 97 | 9052.67
2021-03 | P01 | Site 1 (synthetic) | 306 | 28531.31
2021-03 | P02 | Site 1 (synthetic) | 129 | 12046.96
2021-03 | P03 | Site 1 (synthetic) | 118 | 10968.55
2021-03 | P04 | Site 2 (synthetic) | 110 | 10234.33
2021-03 | P05 | Site 2 (synthetic) | 137 | 12791.18
2021-03 | P06 | Site 4 (synthetic) | 144 | 13420.66
2021-03 | P09 | Site 3 (synthetic) | 115 | 10740.23
2021-03 | P13 | Site 4 (synthetic) | 96 | 8979.98
2021-03 | P14 | Site 5 (synthetic) | 104 | 9676.24
2021-03 | P17 | Site 5 (synthetic) | 100 | 9283.49
2021-03 | P18 | Site 6 (synthetic) | 101 | 9425.06
2021-03 | P21 | Site 6 (synthetic) | 98 | 9097.91
2021-04 | P01 | Site 1 (synthetic) | 308 | 28673.97
2021-04 | P02 | Site 1 (synthetic) | 130 | 12107.19
2021-04 | P03 | Site 1 (synthetic) | 118 | 11023.39
2021-04 | P04 | Site 2 (synthetic) | 110 | 10285.50
2021-04 | P05 | Site 2 (synthetic) | 138 | 12855.13
2021-04 | P06 | Site 4 (synthetic) | 145 | 13487.77
2021-04 | P09 | Site 3 (synthetic) | 116 | 10793.93
2021-04 | P13 | Site 4 (synthetic) | 97 | 9024.88
2021-04 | P14 | Site 5 (synthetic) | 104 | 9724.62
2021-04 | P17 | Site 5 (synthetic) | 100 | 9329.91
2021-04 | P18 | Site 6 (synthetic) | 102 | 9472.18
2021-04 | P21 | Site 6 (synthetic) | 98 | 9143.41
2021-05 | P01 | Site 1 (synthetic) | 309 | 28817.34
2021-05 | P02 | Site 1 (synthetic) | 131 | 12167.73
2021-05 | P03 | Site 1 (synthetic) | 119 | 11078.51
2021-05 | P04 | Site 2 (synthetic) | 111 | 10336.93
2021-05 | P05 | Site 2 (synthetic) | 139 | 12919.41
2021-05 | P06 | Site 4 (synthetic) | 145 | 13555.21
2021-05 | P09 | Site 3 (synthetic) | 116 | 10847.90
2021-05 | P13 | Site 4 (synthetic) | 97 | 9070.00
2021-05 | P14 | Site 5 (synthetic) | 105 | 9773.24
2021-05 | P17 | Site 5 (synthetic) | 101 | 9376.56
2021-05 | P18 | Site 6 (synthetic) | 102 | 9519.54
2021-05 | P21 | Site 6 (synthetic) | 99 | 9189.12
… 768 more rows in clinician-collections.csv
---page---
referrals.csv — Visits by referral source and month, from the schedule export

month | referral_source | source_type | visits | new_patients
2025-10 | Harbourside Hospital orthopaedics (synthetic) | hospital | 673 | 148
2025-10 | Northgate Physician Group (synthetic) | physician group | 151 | 33
2025-10 | Bluepoint plan network (synthetic) | plan | 104 | 23
2025-10 | Self-referral | self-referral | 233 | 51
2025-11 | Harbourside Hospital orthopaedics (synthetic) | hospital | 679 | 149
2025-11 | Northgate Physician Group (synthetic) | physician group | 152 | 33
2025-11 | Bluepoint plan network (synthetic) | plan | 105 | 23
2025-11 | Self-referral | self-referral | 235 | 52
2025-12 | Harbourside Hospital orthopaedics (synthetic) | hospital | 702 | 154
2025-12 | Northgate Physician Group (synthetic) | physician group | 157 | 35
2025-12 | Bluepoint plan network (synthetic) | plan | 109 | 24
2025-12 | Self-referral | self-referral | 243 | 53
2026-01 | Harbourside Hospital orthopaedics (synthetic) | hospital | 670 | 147
2026-01 | Northgate Physician Group (synthetic) | physician group | 150 | 33
2026-01 | Bluepoint plan network (synthetic) | plan | 104 | 23
2026-01 | Self-referral | self-referral | 231 | 51
2026-02 | Harbourside Hospital orthopaedics (synthetic) | hospital | 663 | 146
2026-02 | Northgate Physician Group (synthetic) | physician group | 149 | 33
2026-02 | Bluepoint plan network (synthetic) | plan | 103 | 23
2026-02 | Self-referral | self-referral | 228 | 50
2026-03 | Harbourside Hospital orthopaedics (synthetic) | hospital | 684 | 150
2026-03 | Northgate Physician Group (synthetic) | physician group | 153 | 34
2026-03 | Bluepoint plan network (synthetic) | plan | 106 | 23
2026-03 | Self-referral | self-referral | 237 | 52
2026-04 | Harbourside Hospital orthopaedics (synthetic) | hospital | 688 | 151
2026-04 | Northgate Physician Group (synthetic) | physician group | 154 | 34
2026-04 | Bluepoint plan network (synthetic) | plan | 107 | 24
2026-04 | Self-referral | self-referral | 238 | 52
2026-05 | Harbourside Hospital orthopaedics (synthetic) | hospital | 673 | 148
2026-05 | Northgate Physician Group (synthetic) | physician group | 151 | 33
2026-05 | Bluepoint plan network (synthetic) | plan | 104 | 23
2026-05 | Self-referral | self-referral | 233 | 51
2026-06 | Harbourside Hospital orthopaedics (synthetic) | hospital | 679 | 149
2026-06 | Northgate Physician Group (synthetic) | physician group | 152 | 33
2026-06 | Bluepoint plan network (synthetic) | plan | 105 | 23
2026-06 | Self-referral | self-referral | 235 | 52
2026-07 | Harbourside Hospital orthopaedics (synthetic) | hospital | 678 | 149
2026-07 | Northgate Physician Group (synthetic) | physician group | 152 | 33
2026-07 | Bluepoint plan network (synthetic) | plan | 105 | 23
2026-07 | Self-referral | self-referral | 234 | 51
2026-08 | Harbourside Hospital orthopaedics (synthetic) | hospital | 700 | 154
2026-08 | Northgate Physician Group (synthetic) | physician group | 157 | 35
2026-08 | Bluepoint plan network (synthetic) | plan | 109 | 24
2026-08 | Self-referral | self-referral | 241 | 53
2026-09 | Harbourside Hospital orthopaedics (synthetic) | hospital | 670 | 147
2026-09 | Northgate Physician Group (synthetic) | physician group | 150 | 33
2026-09 | Bluepoint plan network (synthetic) | plan | 104 | 23
2026-09 | Self-referral | self-referral | 232 | 51
---page---
credentialing-register.csv — Credentialing register: a licence per pseudonymous provider

credential_ref | provider_ref | kind | jurisdiction | issuer | status | expires_on
CR-0101 | P01 | state_licence | England | England dental board (synthetic) | active | 2027-01-28
CR-0201 | P02 | state_licence | England | England dental board (synthetic) | active | 2028-02-28
CR-0301 | P03 | state_licence | England | England dental board (synthetic) | active | 2027-03-28
CR-0401 | P04 | state_licence | England | England dental board (synthetic) | active | 2028-04-28
CR-0501 | P05 | state_licence | England | England dental board (synthetic) | active | 2027-05-28
CR-0601 | P06 | state_licence | England | England dental board (synthetic) | active | 2028-06-28
CR-0701 | P09 | state_licence | England | England dental board (synthetic) | active | 2027-07-28
CR-0801 | P13 | state_licence | England | England physiotherapy board (synthetic) | active | 2028-08-28
CR-0901 | P14 | state_licence | England | England physiotherapy board (synthetic) | active | 2027-09-28
CR-1001 | P17 | state_licence | England | England physiotherapy board (synthetic) | active | 2028-10-28
CR-1101 | P18 | state_licence | England | England physiotherapy board (synthetic) | active | 2027-11-28
CR-1201 | P21 | state_licence | England | England physiotherapy board (synthetic) | active | 2028-12-28
---page---
payer-contracts.csv — Payer contract and enrolment register

contract_id | payer | payer_class | effective_on | expires_on | auto_renews
BP-2023 | Insurer Bluepoint (synthetic) | commercial | 2023-01-01 | 2028-12-31 | yes
HG-2024 | Insurer Harrowgate (synthetic) | commercial | 2024-07-01 | 2029-06-30 | no
GS-ENR-118 | Government scheme (synthetic) | medicaid | 2019-04-01 |  | no
---page---
pnl.csv — Profit and loss by fiscal year, FY2021 to FY2025

Line | FY2021 | FY2022 | FY2023 | FY2024 | FY2025
Net patient service revenue | 1773295.79 | 1882668.81 | 1998787.70 | 2123864.76 | 2271663.84
Other operating revenue | 6683.40 | 6896.70 | 7110.00 | 7323.30 | 7536.60
Cost of care: clinical staff | 729791.47 | 774721.86 | 822418.06 | 873787.10 | 934472.18
Clinical and dental supplies | 80099.06 | 105815.67 | 136401.04 | 179019.80 | 234757.65
Laboratory fees | 55179.35 | 58576.53 | 62182.83 | 66066.83 | 68376.01
Rent and occupancy | 135278.42 | 141717.41 | 148436.43 | 155576.73 | 164102.43
General and administrative | 266996.88 | 251312.21 | 236695.93 | 219512.37 | 193732.04
