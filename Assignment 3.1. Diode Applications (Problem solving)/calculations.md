# Calculations — Diode Applications (Week 3–4)

## Core Assumptions and Device Models

* **Thermal Voltage Formula:** $V_T = \frac{kT}{q}$
* **Approximate Diode Model:**
    * **Silicon (Si) ON:** $V_D \approx 0.7\text{ V}$
    * **Silicon (Si) OFF:** Acts as an open circuit
    * **GaAs Diode ON:** $V_D \approx 1.2\text{ V}$ (Typical)
* **Ideal Diode Model:**
    * **ON:** $V_D = 0\text{ V}$
    * **OFF:** Open circuit

---

## 1(a) Calculating Thermal Voltage ($V_T$) at 25°C

Using the formula: $V_T = \frac{kT}{q}$

**Parameters:**
* $k = 1.38 \times 10^{-23}\text{ J/K}$ (Boltzmann constant)
* $q = 1.60 \times 10^{-19}\text{ C}$ (Elementary charge)
* $T = 25^\circ\text{C} + 273 = 298\text{ K}$ (Absolute temperature)

**Calculation:**
$V_T = \frac{(1.38 \times 10^{-23})(298)}{1.60 \times 10^{-19}} \approx 0.0257\text{ V}$

**Result:** $\boxed{V_T \approx 25.7\text{ mV}}$

---

## 1(b) Determining Diode Current via Shockley Equation

**Given Values:**
* $I_S = 40\text{ nA} = 40 \times 10^{-9}\text{ A}$
* $n = 2$
* $V_D = 0.5\text{ V}$
* $V_T = 0.0257\text{ V}$

**Formula:** $I_D = I_S \left( e^{\frac{V_D}{n V_T}} - 1 \right)$

**Step-by-step:**
1. $n V_T = 2(0.0257) = 0.0514\text{ V}$
2. $\frac{V_D}{n V_T} = \frac{0.5}{0.0514} \approx 9.73$
3. $I_D \approx 40 \times 10^{-9} (e^{9.73} - 1) \approx 40 \times 10^{-9} (16800) \approx 6.73 \times 10^{-4}\text{ A}$

**Result:** $\boxed{I_D \approx 0.673\text{ mA}}$

---

## 2) Boylestad Chapter 2, Problem 4

**Circuit Specs:** $E = 30\text{ V}$, Silicon diode in series with $R = 1.5\text{ k}\Omega$.

### (a) Using Approximate Model (Si)
Since the diode is forward-biased, it is **ON**.
* $V_D \approx 0.7\text{ V}$
* $V_R = E - V_D = 30 - 0.7 = 29.3\text{ V}$
* $I_D = \frac{V_R}{R} = \frac{29.3}{1500} \approx 19.53\text{ mA}$

### (b) Using Ideal Model
* $V_D = 0\text{ V}$
* $V_R = 30\text{ V}$
* $I_D = \frac{30}{1500} = 20\text{ mA}$

**Comparison:** The results are very similar because the source voltage ($30\text{ V}$) is significantly larger than the diode drop ($0.7\text{ V}$).

---

## 3) Boylestad Chapter 2, Problem 5 — Approximate Model

**Part (a):** Diode is reverse-biased. Result: $\boxed{I = 0\text{ A}}$

**Part (b):** With a $-20\text{ V}$ source and an ON diode:
* Node before resistor: $V \approx -20 + 0.7 = -19.3\text{ V}$
* Current through $10\text{ }\Omega$ branch: $I_{10} = \frac{-19.3}{10} = 1.93\text{ A}$
* Current through $20\text{ }\Omega$ branch: $I_{20} = \frac{-19.3}{20} = 0.965\text{ A}$
* **Total Current:** $I = 1.93 + 0.965 \approx \boxed{2.90\text{ A}}$

---

## 4) Boylestad Chapter 2, Problem 11

**Part (a):** Parallel Si ($0.7\text{ V}$) and GaAs ($1.2\text{ V}$) diodes. The Silicon diode conducts first.
* $V_o = 1 - 0.7 = 0.3\text{ V}$
* $I = \frac{0.3}{1000} = \boxed{0.3\text{ mA}}$

**Part (b):** Circuit with $+16\text{ V}$ source and two Si drops.
* $V_o = 16 - (0.7 + 0.7) = 14.6\text{ V}$
* Resistor is between $V_o$ and $-4\text{ V}$ node.
* $I = \frac{14.6 - (-4)}{4700} = \frac{18.6}{4700} \approx \boxed{3.96\text{ mA}}$
