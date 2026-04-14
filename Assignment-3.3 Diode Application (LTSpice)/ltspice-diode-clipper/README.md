# LTspice Diode Clipper Circuit

## Student Information
- **Name:** Md Mohiuddin Mollah
- **Student ID:** s2312633

## Assignment Overview
This assignment uses LTspice to simulate the given diode circuit and study its waveform behavior.  
The repository includes the LTspice schematic file, screenshots of the schematic and simulation result, and a short analysis of the observed output.

## Files Included
- `diode_clipper.asc` – LTspice schematic file
- `schematic_window.png` – screenshot of the LTspice schematic window
- `simulation_plot.png` – screenshot of the LTspice simulation result
- `README.md` – explanation and analysis

## Circuit Description
The circuit contains:
- an AC voltage source
- a 1 kΩ series resistor
- a silicon diode
- a 1 kΩ load resistor

The AC input source is set to a peak amplitude of 10 V and a reasonable frequency such as 50 Hz or 60 Hz.  
Transient analysis is used to observe the input and output waveforms over time.

## Simulation Setup
For the simulation:
- the AC source peak amplitude is set to **10 V**
- a transient analysis is used
- the stop time is set long enough to show at least two complete cycles of the input signal
- the input voltage `vi` and output voltage `vo` are plotted

## Waveforms Observed
The following waveforms are observed in LTspice:
- **Input voltage (`vi`)**
- **Output voltage (`vo`)**

## Analysis
When the diode is not conducting, the output voltage is mainly determined by the resistor network and follows the input waveform in a reduced form.  
When the diode becomes forward biased, it starts conducting and limits the output voltage, so the waveform becomes clipped.

Because the circuit uses a silicon diode, the clipping begins near the diode forward voltage, which is approximately **0.7 V**.  
This causes one part of the waveform to be limited, while the other part follows the normal resistor-divider behavior.

## What the Plot Shows
The simulation plot shows the original sinusoidal input and the modified output waveform.  
The output is different from the input because the diode changes the circuit behavior depending on whether it is OFF or ON during different parts of the AC cycle.

## Screenshots

### 1. LTspice Schematic Window
Add the screenshot here.

**[Insert schematic window screenshot here]**

### 2. Simulation Plot
Add the screenshot here.

**[Insert simulation plot screenshot here]**

## Conclusion
This simulation helps explain how a diode clipper circuit changes an AC waveform.  
By using LTspice, it is possible to compare the input and output signals and understand how the diode affects the circuit during different parts of the cycle.
