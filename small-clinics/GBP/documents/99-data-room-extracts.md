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
2023-01 | Insurer Bluepoint (synthetic) | commercial | 711 | 35 | 86867.41 | 66311.00 | 104103.73
2023-01 | Insurer Harrowgate (synthetic) | commercial | 419 | 20 | 51731.57 | 39489.75 | 61383.59
2023-01 | Government scheme (synthetic) | medicaid | 487 | 23 | 37294.49 | 28469.08 | 44562.01
2023-01 | Patients — self-pay (synthetic) | self_pay | 366 | 18 | 36371.82 | 27764.75 | 42684.25
2023-02 | Insurer Bluepoint (synthetic) | commercial | 708 | 34 | 87301.74 | 66642.55 | 103693.79
2023-02 | Insurer Harrowgate (synthetic) | commercial | 426 | 20 | 51990.23 | 39687.20 | 61136.41
2023-02 | Government scheme (synthetic) | medicaid | 487 | 24 | 37480.97 | 28611.43 | 45051.14
2023-02 | Patients — self-pay (synthetic) | self_pay | 371 | 18 | 36553.69 | 27903.58 | 43330.55
2023-03 | Insurer Bluepoint (synthetic) | commercial | 718 | 35 | 87738.25 | 66975.76 | 105459.07
2023-03 | Insurer Harrowgate (synthetic) | commercial | 431 | 20 | 52250.18 | 39885.63 | 62555.84
2023-03 | Government scheme (synthetic) | medicaid | 496 | 25 | 37668.37 | 28754.48 | 44830.32
2023-03 | Patients — self-pay (synthetic) | self_pay | 367 | 17 | 36736.46 | 28043.10 | 43982.24
2023-04 | Insurer Bluepoint (synthetic) | commercial | 716 | 34 | 88176.94 | 67310.64 | 102958.18
2023-04 | Insurer Harrowgate (synthetic) | commercial | 426 | 21 | 52511.43 | 40085.06 | 61749.30
2023-04 | Government scheme (synthetic) | medicaid | 492 | 24 | 37856.72 | 28898.26 | 44337.19
2023-04 | Patients — self-pay (synthetic) | self_pay | 374 | 18 | 36920.14 | 28183.31 | 43458.89
2023-05 | Insurer Bluepoint (synthetic) | commercial | 718 | 35 | 88617.83 | 67647.20 | 105047.11
2023-05 | Insurer Harrowgate (synthetic) | commercial | 435 | 21 | 52773.99 | 40285.49 | 62058.05
2023-05 | Government scheme (synthetic) | medicaid | 496 | 24 | 38046.00 | 29042.75 | 44784.15
2023-05 | Patients — self-pay (synthetic) | self_pay | 373 | 18 | 37104.74 | 28324.23 | 43280.73
2023-06 | Insurer Bluepoint (synthetic) | commercial | 725 | 34 | 89060.91 | 67985.43 | 104517.67
2023-06 | Insurer Harrowgate (synthetic) | commercial | 430 | 20 | 53037.87 | 40486.92 | 61991.50
2023-06 | Government scheme (synthetic) | medicaid | 500 | 24 | 38236.23 | 29187.96 | 45596.70
2023-06 | Patients — self-pay (synthetic) | self_pay | 374 | 18 | 37290.26 | 28465.85 | 44468.64
2023-07 | Insurer Bluepoint (synthetic) | commercial | 731 | 35 | 89506.22 | 68325.36 | 107266.14
2023-07 | Insurer Harrowgate (synthetic) | commercial | 434 | 21 | 53303.05 | 40689.35 | 62427.69
2023-07 | Government scheme (synthetic) | medicaid | 499 | 24 | 38427.41 | 29333.90 | 45324.12
2023-07 | Patients — self-pay (synthetic) | self_pay | 379 | 19 | 37476.72 | 28608.18 | 45046.03
2023-08 | Insurer Bluepoint (synthetic) | commercial | 731 | 36 | 89953.76 | 68666.99 | 107269.86
2023-08 | Insurer Harrowgate (synthetic) | commercial | 439 | 21 | 53569.57 | 40892.80 | 63754.84
2023-08 | Government scheme (synthetic) | medicaid | 507 | 24 | 38619.55 | 29480.57 | 45413.54
2023-08 | Patients — self-pay (synthetic) | self_pay | 376 | 18 | 37664.10 | 28751.22 | 44557.62
2023-09 | Insurer Bluepoint (synthetic) | commercial | 737 | 36 | 90403.52 | 69010.32 | 105879.18
2023-09 | Insurer Harrowgate (synthetic) | commercial | 438 | 21 | 53837.41 | 41097.26 | 63053.52
2023-09 | Government scheme (synthetic) | medicaid | 507 | 25 | 38812.64 | 29627.97 | 46605.81
2023-09 | Patients — self-pay (synthetic) | self_pay | 379 | 18 | 37852.42 | 28894.98 | 44287.33
2023-10 | Insurer Bluepoint (synthetic) | commercial | 743 | 36 | 90855.53 | 69355.37 | 106623.75
2023-10 | Insurer Harrowgate (synthetic) | commercial | 439 | 22 | 54106.60 | 41302.75 | 63881.38
2023-10 | Government scheme (synthetic) | medicaid | 506 | 24 | 39006.70 | 29776.11 | 45499.26
2023-10 | Patients — self-pay (synthetic) | self_pay | 386 | 18 | 38041.68 | 29039.45 | 44508.77
2023-11 | Insurer Bluepoint (synthetic) | commercial | 742 | 35 | 91309.82 | 69702.15 | 108454.44
2023-11 | Insurer Harrowgate (synthetic) | commercial | 448 | 22 | 54377.13 | 41509.26 | 63878.82
2023-11 | Government scheme (synthetic) | medicaid | 517 | 24 | 39201.74 | 29924.99 | 47073.04
2023-11 | Patients — self-pay (synthetic) | self_pay | 389 | 18 | 38231.89 | 29184.65 | 45908.45
2023-12 | Insurer Bluepoint (synthetic) | commercial | 745 | 36 | 91766.36 | 70050.66 | 109974.74
2023-12 | Insurer Harrowgate (synthetic) | commercial | 447 | 22 | 54649.02 | 41716.81 | 65233.67
2023-12 | Government scheme (synthetic) | medicaid | 513 | 24 | 39397.75 | 30074.62 | 46095.37
2023-12 | Patients — self-pay (synthetic) | self_pay | 390 | 19 | 38423.05 | 29330.57 | 45364.48
2024-01 | Insurer Bluepoint (synthetic) | commercial | 752 | 37 | 92225.19 | 70400.91 | 108777.18
2024-01 | Insurer Harrowgate (synthetic) | commercial | 447 | 21 | 54922.26 | 41925.39 | 64844.40
2024-01 | Government scheme (synthetic) | medicaid | 513 | 24 | 39594.74 | 30224.99 | 47169.84
2024-01 | Patients — self-pay (synthetic) | self_pay | 390 | 19 | 38615.16 | 29477.22 | 45728.48
2024-02 | Insurer Bluepoint (synthetic) | commercial | 757 | 37 | 92686.33 | 70752.92 | 109979.65
2024-02 | Insurer Harrowgate (synthetic) | commercial | 451 | 22 | 55196.88 | 42135.02 | 65756.91
2024-02 | Government scheme (synthetic) | medicaid | 516 | 24 | 39792.72 | 30376.12 | 47170.08
2024-02 | Patients — self-pay (synthetic) | self_pay | 388 | 19 | 38808.24 | 29624.61 | 46462.65
2024-03 | Insurer Bluepoint (synthetic) | commercial | 761 | 36 | 93149.75 | 71106.68 | 109316.13
2024-03 | Insurer Harrowgate (synthetic) | commercial | 458 | 22 | 55472.85 | 42345.69 | 64771.85
2024-03 | Government scheme (synthetic) | medicaid | 522 | 24 | 39991.68 | 30528.00 | 46932.34
2024-03 | Patients — self-pay (synthetic) | self_pay | 393 | 19 | 39002.28 | 29772.73 | 45725.04
… 120 more rows in remittances.csv
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
clinician-collections.csv — Collections by clinician and month, pseudonymous, from the practice-management system

month | provider_ref | site | visits | collected
2025-10 | P01 | Site 1 (synthetic) | 188 | 37883.36
2025-10 | P02 | Site 1 (synthetic) | 165 | 15669.66
2025-10 | P03 | Site 1 (synthetic) | 247 | 16604.52
2025-10 | P04 | Site 2 (synthetic) | 202 | 13585.52
2025-10 | P05 | Site 2 (synthetic) | 165 | 15669.66
2025-10 | P06 | Site 4 (synthetic) | 202 | 19151.81
2025-10 | P09 | Site 3 (synthetic) | 180 | 12076.02
2025-10 | P13 | Site 4 (synthetic) | 144 | 9643.59
2025-10 | P14 | Site 5 (synthetic) | 215 | 14465.39
2025-10 | P17 | Site 5 (synthetic) | 197 | 13259.94
2025-10 | P18 | Site 6 (synthetic) | 215 | 14465.39
2025-10 | P21 | Site 6 (synthetic) | 144 | 9643.60
2025-11 | P01 | Site 1 (synthetic) | 185 | 37601.01
2025-11 | P02 | Site 1 (synthetic) | 169 | 15988.70
2025-11 | P03 | Site 1 (synthetic) | 217 | 14555.23
2025-11 | P04 | Site 2 (synthetic) | 199 | 13342.29
2025-11 | P05 | Site 2 (synthetic) | 186 | 17587.57
2025-11 | P06 | Site 4 (synthetic) | 186 | 17587.56
2025-11 | P09 | Site 3 (synthetic) | 217 | 14555.23
2025-11 | P13 | Site 4 (synthetic) | 177 | 11874.89
2025-11 | P14 | Site 5 (synthetic) | 212 | 14249.87
2025-11 | P17 | Site 5 (synthetic) | 159 | 10687.40
2025-11 | P18 | Site 6 (synthetic) | 212 | 14249.87
2025-11 | P21 | Site 6 (synthetic) | 159 | 10687.41
2025-12 | P01 | Site 1 (synthetic) | 192 | 38750.04
2025-12 | P02 | Site 1 (synthetic) | 150 | 14247.24
2025-12 | P03 | Site 1 (synthetic) | 228 | 15340.75
2025-12 | P04 | Site 2 (synthetic) | 166 | 11156.91
2025-12 | P05 | Site 2 (synthetic) | 188 | 17809.05
2025-12 | P06 | Site 4 (synthetic) | 207 | 19589.95
2025-12 | P09 | Site 3 (synthetic) | 249 | 16735.35
2025-12 | P13 | Site 4 (synthetic) | 174 | 11699.42
2025-12 | P14 | Site 5 (synthetic) | 174 | 11699.42
2025-12 | P17 | Site 5 (synthetic) | 174 | 11699.42
2025-12 | P18 | Site 6 (synthetic) | 196 | 13161.85
2025-12 | P21 | Site 6 (synthetic) | 218 | 14624.27
2026-01 | P01 | Site 1 (synthetic) | 190 | 38675.45
2026-01 | P02 | Site 1 (synthetic) | 213 | 20239.18
2026-01 | P03 | Site 1 (synthetic) | 251 | 16839.72
2026-01 | P04 | Site 2 (synthetic) | 188 | 12629.79
2026-01 | P05 | Site 2 (synthetic) | 142 | 13492.79
2026-01 | P06 | Site 4 (synthetic) | 196 | 18552.58
2026-01 | P09 | Site 3 (synthetic) | 209 | 14033.10
2026-01 | P13 | Site 4 (synthetic) | 217 | 14602.27
2026-01 | P14 | Site 5 (synthetic) | 163 | 10951.71
2026-01 | P17 | Site 5 (synthetic) | 217 | 14602.27
2026-01 | P18 | Site 6 (synthetic) | 199 | 13385.42
2026-01 | P21 | Site 6 (synthetic) | 145 | 9734.85
2026-02 | P01 | Site 1 (synthetic) | 187 | 38408.79
2026-02 | P02 | Site 1 (synthetic) | 151 | 14341.48
2026-02 | P03 | Site 1 (synthetic) | 210 | 14079.67
2026-02 | P04 | Site 2 (synthetic) | 229 | 15359.64
2026-02 | P05 | Site 2 (synthetic) | 202 | 19121.97
2026-02 | P06 | Site 4 (synthetic) | 202 | 19121.98
2026-02 | P09 | Site 3 (synthetic) | 210 | 14079.66
2026-02 | P13 | Site 4 (synthetic) | 213 | 14332.15
2026-02 | P14 | Site 5 (synthetic) | 160 | 10749.11
2026-02 | P17 | Site 5 (synthetic) | 213 | 14332.15
2026-02 | P18 | Site 6 (synthetic) | 196 | 13137.80
2026-02 | P21 | Site 6 (synthetic) | 160 | 10749.10
… 84 more rows in clinician-collections.csv
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
pnl.csv — Profit and loss by fiscal year, FY2023 to FY2025

Line | FY2023 | FY2024 | FY2025
Net patient service revenue | 1998787.70 | 2123864.76 | 2271663.84
Other operating revenue | 7110.00 | 7323.30 | 7536.60
Cost of care: clinical staff | 822418.06 | 873787.10 | 934472.18
Clinical and dental supplies | 136401.04 | 179019.80 | 234757.65
Laboratory fees | 62182.83 | 66066.83 | 68376.01
Rent and occupancy | 148436.43 | 155576.73 | 164102.43
General and administrative | 236695.93 | 219512.37 | 193732.04
