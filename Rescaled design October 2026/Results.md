**Device:** C1 = 95 fF, CA = 228 fF, C2 = 95 fF, CB = 228 fF, C3 = 98 fF, C1A = 5.36 fF, CA2 = 5.36 fF, C2B = 5.36 fF, CB3 = 5.36 fF, C12 = 0.125 fF, C23 = 0.125 fF

**Model:** site-basis Hamiltonian, (6, 8, 6, 8, 6) levels per transmon (Q1, cA, Q2, cB, Q3), Taylor 8, 20 eigenlevels; Hz; dressed site frequencies; g = H12 so 2g = 2H (signed); static two-state pair estimates, holds exclude ramps; inductances are MODEL values (the flux map is the hardware calibration).

## Target 3.65 GHz

| Quantity | idle | gate 12 | 100 ns hold | 50 ns hold | pair null |
|---|---:|---:|---:|---:|---:|
| Lj1 [nH] | 16.959254 | 16.959254 | 16.959254 | 16.959254 | 16.959254 |
| Lj2 [nH] | 16.156095 | 16.156095 | 16.156095 | 16.156095 | 16.144568 |
| Lj3 [nH] | 16.521078 | 16.521078 | 16.521078 | 16.521078 | 19.445102 |
| LjA [nH] | 3.929715 | 4.641870 | 5.304095 | 5.950161 | 3.929712 |
| LjB [nH] | 3.929732 | 3.929732 | 3.929732 | 3.929732 | 4.843851 |
| fQ1 [GHz] | 3.650000 | 3.648952 | 3.647423 | 3.644849 | 3.650000 |
| fQ2 [GHz] | 3.650000 | 3.649010 | 3.647565 | 3.645133 | 3.650000 |
| fQ3 [GHz] | 3.650000 | 3.650000 | 3.650000 | 3.650000 | 3.347952 |
| fcA [GHz] | 5.125955 | 4.712281 | 4.406456 | 4.161354 | 5.125954 |
| fcB [GHz] | 5.125764 | 5.125758 | 5.125749 | 5.125730 | 4.610447 |
| 2g12 [kHz] | +0.0121 | -2031.2392 | -5000.0016 | -9999.9999 | +0.0189 |
| ZZ12 [kHz] | -0.541933 | +0.000002 | +31.088884 | +108.435112 | -0.540010 |
| 2g23 [kHz] | +0.0106 | +2.3899 | +5.8277 | +11.5018 | -1528.9528 |
| ZZ23 [kHz] | -0.526133 | -0.512405 | -0.491864 | -0.456119 | -6.803999 |
| 2g13 [kHz] | -0.0006 | +2.4403 | +5.9714 | +11.8036 | +0.9369 |
| ZZ13 [kHz] | +0.000004 | -0.000070 | -0.000339 | -0.001442 | -0.000016 |
| ZZ12 angle rate at rest [deg/us] | -0.19510 | +0.00000 | +11.19200 | +39.03664 | -0.19440 |
| ZZ23 angle rate at rest [deg/us] | -0.18941 | -0.18447 | -0.17707 | -0.16420 | -2.44944 |
| ZZ13 angle rate at rest [deg/us] | +0.00000 | -0.00003 | -0.00012 | -0.00052 | -0.00001 |
| ZZ12 angle rate at rest [rad/us] | -0.0034051 | +0.0000000 | +0.1953372 | +0.6813179 | -0.0033930 |
| three-qubit spread [MHz] | 0.000024 | 1.047839 | 2.577191 | 5.150833 | (Q3 parked) 302.048 |
| pair detuning fQ1 - fQ2 [kHz] | -0.024 | -57.847 | -142.077 | -283.546 | -0.038 |
| nominal hold 1/(4 g12) [ns] | - | 246.155 | 100.000 | 50.000 | - |
| first transfer maximum [ns] | - | 246.055 | 99.960 | 49.980 | - |
| maximum transfer [%] | - | 99.9190 | 99.9193 | 99.9197 | - |
| ZZ12 phase over the hold [deg] | - | +0.0000 | +1.1192 | +1.9518 | - |
| ZZ12 phase over the hold [rad] | - | +0.000000 | +0.019534 | +0.034066 | - |
| fold defect (1-exc / 2-exc) | 0.0129 / 0.0188 | 0.0164 / 0.0228 | 0.0238 / 0.0305 | 0.0412 / 0.0484 | 0.0162 / 0.0223 |
| static criteria | PASS | FAIL: Three-qubit frequency spread <1 MHz | FAIL: Three-qubit frequency spread <1 MHz (reported, not enforced, as in the report) | FAIL: Three-qubit frequency spread <1 MHz (reported, not enforced, as in the report) | PASS |

Hold / angle trade-off on the active branch (nominal hold 1/(4|g12|) -> ZZ12 angle accumulated over it; no ZZ cap is imposed):

| nominal hold [ns] | fcA [GHz] | 2g12 [MHz] | ZZ12 [kHz] | angle [deg] | angle [rad] | spread [MHz] | fold defect (2-exc) |
|---:|---:|---:|---:|---:|---:|---:|---:|
| 246.2 | 4.7123 | -2.0312 | +0.000 | +0.000 | +0.00000 | 1.048 | 0.023 |
| 211.8 | 4.6665 | -2.3604 | +1.956 | +0.149 | +0.00260 | 1.217 | 0.024 |
| 122.1 | 4.4791 | -4.0934 | +18.839 | +0.828 | +0.01446 | 2.110 | 0.028 |
| 100.0 | 4.4065 | -5.0000 | +31.089 | +1.119 | +0.01953 | 2.577 | 0.031 |
| 77.4 | 4.3133 | -6.4594 | +53.737 | +1.497 | +0.02614 | 3.329 | 0.035 |
| 50.7 | 4.1659 | -9.8642 | +106.681 | +1.947 | +0.03398 | 5.081 | 0.048 |
| 50.0 | 4.1614 | -10.0000 | +108.435 | +1.952 | +0.03407 | 5.151 | 0.048 |
| 33.1 | 4.0349 | -15.1218 | +117.513 | +1.399 | +0.02441 | 7.786 | 0.074 |

Pair-null frozen scan, ZZ12 = 0 at: LjA = 3.8871 nH, fcA = 5.1543 GHz, 2g12 = +0.097 MHz (5143 ns); LjA = 4.6381 nH, fcA = 4.7142 GHz, 2g12 = -2.014 MHz (248 ns).
