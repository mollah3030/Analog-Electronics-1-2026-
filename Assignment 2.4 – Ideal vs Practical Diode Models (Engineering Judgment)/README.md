# Assignment 2.4 – Ideal vs Practical Diode Models

This project explores the differences between ideal and practical diode models by utilizing a DC sweep analysis in LTspice.

### The Ideal Diode Model
The ideal diode model acts as a perfect switch, conducting instantly as soon as a positive voltage is applied. It lacks a forward voltage drop (turn-on voltage), and the current spikes almost vertically upon conduction. This simplified behavior makes it an excellent tool for grasping fundamental circuit concepts and performing quick, high-level estimations without worrying about real-world physical constraints.

### The Practical Diode Model
On the other hand, the practical diode model exhibits a clear turn-on voltage, typically around 0.6 V to 0.7 V. Before reaching this threshold, the forward current remains negligible. Once the turn-on voltage is exceeded, the current rises more gradually. This smoothed curve is caused by internal physical factors like carrier recombination and bulk junction resistance.

### Current Behavior Differences
The way current behaves in both models is visibly distinct. While the ideal diode shows an extremely steep current rise, the practical diode's current slope is restricted by its internal series resistance. Accounting for these specific effects is crucial when designing actual circuits where realistic voltage drops and power dissipation must be calculated.

### When to Use Which Model
Despite their limitations, **ideal diode models** remain highly valuable. They are frequently used to streamline complex math and teach core electronics principles, making them perfect for initial drafting phases and academic learning.

Nevertheless, when a design requires highly accurate voltage tolerances, exact power loss calculations, and true-to-life performance metrics, the ideal model falls short. In these practical scenarios, employing a **practical diode model** is absolutely necessary to achieve reliable, realistic simulation results.
