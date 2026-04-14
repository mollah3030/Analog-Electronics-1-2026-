# LTspice Op-Amp Behaviors

## Student Information
- **Name:** Md Mohiuddin Mollah
- **Student ID:** s2312633

## Tool and Submission
- **Tool:** LTspice and Lab
- **Submission:** One LTspice schematic file (`.asc`) and screenshots of waveforms
- **Submission Platform:** GitHub only

## Goal
The purpose of this lab is to understand basic op-amp behaviors by building and observing three different circuits in LTspice:
1. Open-loop op-amp as a comparator
2. Non-inverting amplifier
3. Inverting amplifier

---

# Task 1 - Open-Loop Op-Amp (Comparator)

## Build
- Op-amp with **±5 V** supply
- `Vin` connected to **(+)**
- `(-)` connected to **GND**
- No feedback
- Input source: `SINE(0 10m 1k)`

## Observe
- Output saturates at **±Vs**
- The op-amp behaves like a **comparator**

## Explanation
In this circuit, the op-amp is used without feedback, so it operates in open-loop mode.  
Because of the very high open-loop gain, even a small difference between the input terminals drives the output quickly to positive or negative saturation.

## Result Screenshot
Add the waveform screenshot here after simulation.

**[Insert Task 1 waveform screenshot here]**

---

# Task 2 - Non-Inverting Amplifier

## Build
- `Vin` connected to **(+)**
- `Rg = 10k` from `(-)` to **GND**
- `Rf = 90k` from `Vout` to `(-)`

## Observe
- Gain ≈ `1 + Rf/Rg ≈ 10`
- No phase inversion

## Explanation
This circuit is a non-inverting amplifier because the input signal is applied to the non-inverting terminal.  
The output remains in phase with the input, and the voltage gain is approximately 10 based on the resistor ratio.

## Result Screenshot
Add the waveform screenshot here after simulation.

**[Insert Task 2 waveform screenshot here]**

---

# Task 3 - Inverting Amplifier

## Build
- `(+)` connected to **GND**
- `Rin = 10k` from `Vin` to `(-)`
- `Rf = 90k` from `Vout` to `(-)`

## Observe
- Gain ≈ `-Rf/Rin ≈ -9`
- `180°` phase inversion

## Explanation
This circuit is an inverting amplifier because the input is applied through a resistor to the inverting terminal, while the non-inverting terminal is grounded.  
The output is amplified and inverted, so it is 180 degrees out of phase with the input signal.

## Result Screenshot
Add the waveform screenshot here after simulation.

**[Insert Task 3 waveform screenshot here]**

---

# Files Included
- `README.md`
- `opamp_behaviors.asc`

---

# Conclusion
This lab helps explain how op-amps behave in different configurations.  
The open-loop circuit acts like a comparator, the non-inverting amplifier gives positive gain without phase inversion, and the inverting amplifier gives negative gain with phase reversal.
