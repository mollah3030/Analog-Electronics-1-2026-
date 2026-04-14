# Zener Diode Voltage Limiting

## Student Information
- **Name:** Md Mohiuddin Mollah
- **Student ID:** s2312633

## Objective
The objective of this assignment is to observe how a Zener diode limits the output voltage under different load conditions.

## Files Included
- `zener_voltage_limiting.asc` – LTspice schematic file
- `README.md` – assignment explanation and result discussion
- `schematic_window.png` – screenshot of the LTspice schematic
- `simulation_100k.png` – output result for 100 kΩ load
- `simulation_10k.png` – output result for 10 kΩ load
- `simulation_1k.png` – output result for 1 kΩ load

## Circuit Description
The circuit contains:
- a **16 V DC source**
- a **1 kΩ series resistor**
- a **10 V Zener diode**
- a load resistor connected in parallel with the Zener diode

The output voltage **Vout** is measured across the load resistor.

## Steps Performed
1. Drew the circuit in LTspice using a DC source, series resistor, Zener diode, and load resistor.
2. Set the input voltage to **16 V** and used a **10 V Zener diode**.
3. Ran **Operating Point Analysis**.
4. Measured the output voltage **Vout** across the load resistor.
5. Changed the load resistor value from **100 kΩ** to **10 kΩ** and then to **1 kΩ**.
6. Recorded how the output voltage changed as the load changed.

## Load Cases

### 1. Load Resistor = 100 kΩ
With a light load, the Zener diode is able to maintain the output voltage close to its Zener voltage.  
The output remains nearly constant because the load current is small and enough current is available for Zener regulation.

### 2. Load Resistor = 10 kΩ
When the load is reduced to 10 kΩ, the load current increases.  
The Zener diode can still regulate the output voltage, but the circuit is under heavier loading than in the 100 kΩ case.

### 3. Load Resistor = 1 kΩ
When the load is changed to 1 kΩ, the current demand becomes much larger.  
In this case, the Zener diode may no longer keep the output voltage perfectly constant, because more current is taken by the load and less current remains for Zener regulation.

## What the Simulation Shows
The simulation shows how the Zener diode works as a voltage limiter.  
For higher load resistance values, the output voltage stays close to the Zener voltage, but when the load resistance becomes smaller, the regulation becomes weaker.

## Short Conclusion
The Zener diode helps keep the output voltage nearly constant, especially when the load is light.  
However, when the load becomes heavier, the output voltage can change because the available current is shared between the load and the Zener diode.

## Answer to the Main Question
**Does the Zener diode keep the output voltage nearly constant? Why?**

Yes, the Zener diode keeps the output voltage nearly constant when it operates in its breakdown region and enough current flows through it.  
If the load current becomes too high, the Zener current decreases, and the output voltage may no longer stay fully constant.

## Screenshots

### 1. LTspice Schematic
Add the screenshot here.

**[Insert schematic screenshot here]**

### 2. Output Result for 100 kΩ Load
Add the screenshot here.

**[Insert 100 kΩ result screenshot here]**

### 3. Output Result for 10 kΩ Load
Add the screenshot here.

**[Insert 10 kΩ result screenshot here]**

### 4. Output Result for 1 kΩ Load
Add the screenshot here.

**[Insert 1 kΩ result screenshot here]**
