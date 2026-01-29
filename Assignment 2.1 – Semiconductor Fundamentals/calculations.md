# Calculations – Question 4

## Question 4(a)  
**Determine the thermal voltage for a diode at a temperature of 25°C.**

**Given:**  
- Temperature, \(T_C = 25^\circ C\)  
- Boltzmann constant, \(k = 1.38 \times 10^{-23}\ \text{J/K}\)  
- Electron charge, \(q = 1.6 \times 10^{-19}\ \text{C}\)

**Formula:**  
\[
V_T = \frac{kT}{q}
\]
\[
T_K = T_C + 273
\]

**Step-by-step:**  
\[
T_K = 25 + 273 = 298\ \text{K}
\]
\[
V_T = \frac{(1.38 \times 10^{-23})(298)}{1.6 \times 10^{-19}}
\]
\[
V_T \approx 0.0257\ \text{V}
\]

**Final Answer:**  
\[
V_T \approx 25.7\ \text{mV}
\]

---

## Question 4(b)  
**For the same diode, find the diode current using the diode equation.**

**Given:**  
- \(I_S = 40\ \text{nA} = 40 \times 10^{-9}\ \text{A}\)  
- \(n = 2\)  
- \(V_T = 0.0257\ \text{V}\)  
- \(V_D = 0.5\ \text{V}\)

**Formula:**  
\[
I_D = I_S\left(e^{\frac{V_D}{nV_T}} - 1\right)
\]

**Step-by-step:**  
\[
\frac{V_D}{nV_T} = \frac{0.5}{2 \times 0.0257} \approx 9.73
\]
\[
I_D = 40 \times 10^{-9}\left(e^{9.73} - 1\right)
\]
\[
e^{9.73} \approx 1.68 \times 10^{4}
\]
\[
I_D \approx 40 \times 10^{-9} \times 1.68 \times 10^{4}
\]
\[
I_D \approx 6.7 \times 10^{-4}\ \text{A} = 0.00067\ \text{A}
\]

**Final Answer:**  
\[
I_D \approx 0.67\ \text{mA}
\]
