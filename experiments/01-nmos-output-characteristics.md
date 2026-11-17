# Experiment 01 — NMOS Output Characteristics

**Status:** Planned — no simulated results recorded.

## Objective
Plot drain current \(I_D\) against drain-source voltage \(V_{DS}\) for several fixed \(V_{GS}\) values.

## Prediction
With \(V_{GS}>V_{TH}\), current initially rises with \(V_{DS}\). At sufficiently large \(V_{DS}\), the ideal long-channel device approaches saturation; non-ideal models may still show a slope.

## LTspice procedure
1. Create a test bench with one NMOS, a DC voltage source from drain to ground and another from gate to ground.
2. Connect source and body to ground for this introductory experiment.
3. Choose and document a MOSFET model. Record \(V_{TH}\), model parameters, and device dimensions if applicable.
4. Use a DC sweep of the drain supply (example: 0 to 5 V) while stepping the gate supply (example: 1, 2, 3, and 4 V).
5. Plot drain current. Check the sign convention: the negative of the drain supply current may be required if measuring current through the voltage source.
6. Export the waveform and save the original LTspice file.

## Suggested comparison
For each gate voltage, find approximate transition voltage \(V_{DS,sat}\approx V_{GS}-V_{TH}\). Describe deviations caused by the chosen transistor model.

## Evidence to add after running
- Circuit file:
- Simulator and version:
- Device model:
- Output plot with units:
- Numerical data:
- Observed operating regions:
- Discrepancies and limitations:
