# MOSFET Characterization — Semiconductor Device Study

**Status: Project initialized — experiments not yet performed.**

This repository is a hands-on electrical-engineering project to study MOSFET operating regions, output and transfer characteristics, and the relationship between simplified theory and SPICE simulation.

It is part of the [Semiconductor Engineering Learning Journey](https://github.com/ZAIDRAR/semiconductor-learning-journey).

## Research questions
1. How does the drain current \(I_D\) change when \(V_{DS}\) increases at fixed \(V_{GS}\)?
2. What changes when the gate voltage \(V_{GS}\) increases?
3. How do cutoff, triode, and saturation regions appear in simulated curves?
4. What are the limitations of a simple MOSFET model?

## Initial experiments

| ID | Experiment | Status |
|---|---|---|
| 01 | [NMOS output characteristics: \(I_D\) versus \(V_{DS}\)](experiments/01-nmos-output-characteristics.md) | Planned |
| 02 | [NMOS transfer characteristics: \(I_D\) versus \(V_{GS}\)](experiments/02-nmos-transfer-characteristics.md) | Planned |
| 03 | Threshold voltage and transconductance estimation | Planned |

## Repository guide

- [Theory](theory/README.md) — physical meaning, simplified equations, limitations
- [Experiments](experiments/README.md) — reproducible protocols and observations
- [SPICE starter simulations](simulations/README.md) — example circuit and instructions
- [Measurements](data/README.md) — how to organize numerical data
- [Plots](plots/README.md) — how to save and label plots
- [Scripts](scripts/README.md) — future plotting or extraction scripts
- [Experiment report template](reports/experiment-template.md)

## Tools
- **LTspice** — graphical circuit simulation and waveform analysis
- **ngspice** — optional open-source SPICE workflow for netlists
- **Python** — optional numerical analysis and visualization

## Getting started
1. Read [MOSFET theory](theory/README.md).
2. Reproduce [Experiment 01](experiments/01-nmos-output-characteristics.md) in LTspice or ngspice.
3. Save the actual circuit/netlist, device model, simulation settings and resulting waveforms.
4. Fill in the experiment report and compare with a theoretical prediction.
5. Update the status table only after the evidence has been uploaded.

**Modeling disclaimer:** The included simple Level-1 NMOS netlist is an educational approximation, *not* a calibrated semiconductor process model or a TCAD result. No simulation output or transistor measurements are claimed yet.

## References
- [ngspice documentation](https://ngspice.sourceforge.io/docs.html)
- [LTspice information](https://www.analog.com/en/resources/design-tools-and-calculators/ltspice-simulator.html)
