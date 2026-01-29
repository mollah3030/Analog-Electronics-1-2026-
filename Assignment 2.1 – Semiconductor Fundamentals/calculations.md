# Calculations (Question 4)

## Q4a) Thermal voltage at 25°C
Given:
- T = 25°C = 298 K
- k = 1.38 × 10^-23 J/K
- q = 1.6 × 10^-19 C

Formula:
V_T = kT / q

Calculation:
V_T = (1.38×10^-23 × 298) / (1.6×10^-19)
V_T ≈ 0.0257 V (≈ 25.7 mV)

## Q4b) Diode current using I_D equation
Given:
- I_S = 40 nA = 40×10^-9 A
- n = 2
- V_D = 0.5 V
- V_T = 0.0257 V

Formula:
I_D = I_S ( e^(V_D/(nV_T)) − 1 )

Compute exponent:
V_D/(nV_T) = 0.5 / (2×0.0257) = 0.5 / 0.0514 ≈ 9.73

So:
I_D = 40×10^-9 ( e^9.73 − 1 )

e^9.73 ≈ 1.68×10^4

I_D ≈ 40×10^-9 × 1.68×10^4
I_D ≈ 6.72×10^-4 A
I_D ≈ 0.672 mA
