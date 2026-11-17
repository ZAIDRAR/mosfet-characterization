# MOSFET Theory Notes

## 1. MOSFET terminals
The n-channel MOSFET has drain (D), gate (G), source (S), and body (B) terminals. Define \(V_{GS}=V_G-V_S\), \(V_{DS}=V_D-V_S\), and \(I_D\) using a consistent sign convention.

## 2. Idealized long-channel regions
For a basic enhancement-mode NMOS with a positive drain-source voltage, neglecting body effect and channel-length modulation:

- **Cutoff:** \(V_{GS}\le V_{TH}\), idealized \(I_D\approx 0\).
- **Triode/linear:** \(V_{GS}>V_{TH}\) and \(0\le V_{DS}<V_{GS}-V_{TH}\).

  \[I_D\approx \mu_n C_{ox}\frac{W}{L}\left[(V_{GS}-V_{TH})V_{DS}-\frac{V_{DS}^2}{2}\right]\]

- **Saturation:** \(V_{GS}>V_{TH}\) and \(V_{DS}\ge V_{GS}-V_{TH}\).

  \[I_D\approx \frac{1}{2}\mu_n C_{ox}\frac{W}{L}(V_{GS}-V_{TH})^2\]

These are first-order equations; actual transistor models can include subthreshold conduction, channel-length modulation, mobility degradation, body effect, short-channel effects, and more.

## 3. Output and transfer curves
- **Output curves:** sweep \(V_{DS}\) while stepping \(V_{GS}\); measure \(I_D\).
- **Transfer curves:** sweep \(V_{GS}\) while holding \(V_{DS}\) at a specified constant value; measure \(I_D\).

## 4. Parameters to explore
- Threshold voltage \(V_{TH}\)
- Transconductance \(g_m = \partial I_D/\partial V_{GS}\) at fixed \(V_{DS}\)
- Output conductance \(g_{ds}=\partial I_D/\partial V_{DS}\) at fixed \(V_{GS}\)

## 5. Important distinction
Circuit SPICE uses compact transistor models. TCAD solves semiconductor-device equations numerically across a physical geometry. A compact-model simulation should not be described as TCAD.
