# MoS₂/BSTO Dual-Gate Field-Effect Transistors

**NTU Final Year Project · Zhang Jinming · Supervisor: Prof. Zheng Liu**

This project investigates van der Waals integration of CVD-grown monolayer MoS₂ with exfoliated mica and nominal Ba₀.₆Sr₀.₄TiO₃ (BSTO) gate dielectrics. I fabricated and electrically characterized a mica back-gated reference, two independently fabricated BSTO back-gated devices, and a BSTO/MoS₂ dual-gated transistor.

My work covered materials preparation and transfer, electrode design, electron-beam lithography, Cr/Au deposition and lift-off, followed by transfer/output measurements and simultaneous gate-current analysis.

## Selected results

| Device / metric | Measurement conditions | Result |
| --- | --- | --- |
| Mica reference: drain-current modulation | V<sub>ds</sub> = 0.1 V; V<sub>g</sub> from −5 to +5 V | I<sub>d</sub> increased from approximately 1.77 pA to 0.944 μA, a measured endpoint change of **5.3 × 10⁵** |
| Dual gate: switching endpoint current ratio | V<sub>bg</sub> = 70 V; V<sub>ds</sub> = 0.5 V; forward V<sub>tg</sub> sweep from −4 to +1 V | Approximately 0.061 pA to 194 nA, giving **3.2 × 10⁶** between the specified sweep endpoints |
| Dual gate: hysteresis width | V<sub>bg</sub> = 70 V; V<sub>ds</sub> = 0.1 V; I<sub>d,ref</sub> = 100 pA | Approximately **0.25 V**, extracted between forward and reverse top-gate sweeps |

The current ratios describe measured sweep endpoints. Sub-picoampere off-state readings make the ratios sensitive to the measurement floor. The hysteresis width is a separate, current-criterion-dependent measurement.

## Device architectures

| Configuration | Gate arrangement | Purpose |
| --- | --- | --- |
| Mica back gate | Local metal gate beneath mica, with MoS₂ above the dielectric | Insulating reference and electrostatic-control comparison |
| BSTO Backgate A | Local metal gate beneath BSTO; multiple source–drain electrode pairs | Compare contact regions and leakage contributions |
| BSTO Backgate B | Independently assembled BSTO back-gated device | Examine sweep direction and drain-bias dependence |
| BSTO dual gate | Local Cr/Au top gate / BSTO / MoS₂ / SiO₂ / conductive-Si global back gate | Apply V<sub>tg</sub> and V<sub>bg</sub> independently and coordinate switching |

The dual-gated device combines a local BSTO top-gate stack with the silicon-substrate back gate. Both gates were used during characterization.

## Fabrication workflow

### 1. Material preparation

Monolayer MoS₂ was grown on SiO₂/Si by CVD in a dual-zone tube furnace, using sulfur at 180 °C, MoO₃ at 750 °C, and argon as the carrier gas. Mica and BSTO flakes were prepared by adhesive-tape-assisted mechanical exfoliation. Optical microscopy identified suitable regions for assembly.

| CVD-grown MoS₂ | Exfoliated mica | Exfoliated BSTO |
| :---: | :---: | :---: |
| <img width="280" alt="Optical micrograph of CVD-grown MoS2" src="https://github.com/user-attachments/assets/91122764-58eb-4382-b444-9f05d2cb36ad" /> | <img width="280" alt="Optical micrograph of exfoliated mica" src="https://github.com/user-attachments/assets/b186c625-bf0b-4b64-8a71-b2dedb4f5b11" /> | <img width="280" alt="Optical micrograph of exfoliated BSTO" src="https://github.com/user-attachments/assets/b0fed329-c3bc-4940-b1d0-2f464c88bbdc" /> |

### 2. PDMS-assisted transfer and assembly

A transparent PDMS stamp supported optical alignment and controlled release. For the back-gated devices, the dielectric was placed over a pre-patterned bottom gate. Water-assisted interfacial delamination enabled MoS₂ pickup from the growth substrate, followed by dry stamping onto mica or BSTO.

For the dual-gated device, MoS₂ was first positioned on SiO₂/Si, and BSTO was transferred above the channel. This sequence left the conductive silicon available as the global back gate and provided the dielectric for a local top gate.

| Transfer platform | Optical alignment and release |
| :---: | :---: |
| <img width="330" alt="PDMS transfer equipment" src="https://github.com/user-attachments/assets/16878f50-e6ad-4c73-8bc6-216d812f8a99" /> | <img width="330" alt="Microscope-assisted PDMS alignment and transfer" src="https://github.com/user-attachments/assets/97605128-49e4-49e3-a28f-3aebbdc53d74" /> |

### 3. Electrode fabrication and process troubleshooting

Electrode patterns were designed in AutoCAD and defined by electron-beam lithography. Electron-beam evaporation deposited **Cr 5 nm / Au 50 nm**, followed by lift-off.

Early fabrication runs showed metal peeling during lift-off. I revised the electrode layout to widen narrow features and increase the contact area, then inspected the resulting patterns optically. This connected mask design and metal adhesion with the requirements of contacting transferred flakes.

| Peeling observed after lift-off | Revised electrode layout |
| :---: | :---: |
| <img width="330" alt="Metal electrode peeling after lift-off" src="https://github.com/user-attachments/assets/40400440-7289-4ff6-ad4a-39d13bd6ace2" /> | <img width="330" alt="Wider electrode features after layout revision" src="https://github.com/user-attachments/assets/23aa55f1-d232-44b9-9d29-fe9491c65f10" /> |

| Mica back-gated device | BSTO back-gated device | BSTO dual-gated device |
| :---: | :---: | :---: |
| <img width="280" alt="Fabricated mica back-gated transistor" src="https://github.com/user-attachments/assets/2ea993a4-be38-4794-967a-95aafa971b21" /> | <img width="280" alt="Fabricated BSTO back-gated transistor" src="https://github.com/user-attachments/assets/0dfd1178-8f97-45e5-bc61-277325b3bbe8" /> | <img width="280" alt="Fabricated BSTO dual-gated transistor with local top gate" src="https://github.com/user-attachments/assets/84f49cad-c599-4a9b-bfe4-a6521fb40b80" /> |

## Electrical characterization

A probe station connected to a Keysight semiconductor parameter analyzer supplied gate and drain–source biases. Transfer measurements recorded I<sub>d</sub> together with gate currents. Output sweeps examined conduction under fixed gate settings. The dual-gate measurements independently varied V<sub>tg</sub> and V<sub>bg</sub>.

### Mica reference: gate control and low leakage

At V<sub>ds</sub> = 0.1 V, the mica reference showed a 5.3 × 10⁵ drain-current change over V<sub>g</sub> = −5 to +5 V. Gate leakage remained approximately 0.13–0.32 pA. At positive gate bias, drain current scaled approximately with drain bias over 1–100 mV.

![Mica transfer measurements at three drain biases and gate leakage](figures/mica-transfer.svg)

*Mica reference, electrode pair 1–2. Transfer sweeps at V<sub>ds</sub> = 1, 10 and 100 mV, with gate-current measurements at 100 mV.*

### BSTO back gates: comparing drain and gate currents

BSTO Backgate A showed non-monotonic transfer responses and substantial gate current at negative gate bias. Different electrode pairs produced different responses. BSTO Backgate B showed sweep separation, trace crossings and a negative-bias upturn that became more prominent at lower drain bias.

Comparing I<sub>d</sub> and I<sub>g</sub>, and repeating measurements at different V<sub>ds</sub>, helped distinguish channel conduction from leakage-related backgrounds. Contact resistance and local channel variation were considered when comparing electrode pairs.

| BSTO Backgate A | BSTO Backgate B |
| :---: | :---: |
| ![BSTO Backgate A transfer and gate leakage](figures/bsto-backgate-a.svg) | ![BSTO Backgate B transfer and gate current](figures/bsto-backgate-b.svg) |

*Both measurements used V<sub>ds</sub> = 0.1 V. Device A was swept from −3 to 0 V and back; device B from −3 to +4 V and back.*

### Coordinated dual-gate control

Increasing positive back-gate bias shifted the top-gate turn-on range towards more negative voltages. The back gate established the operating condition, while the local top gate controlled switching within that condition. Strong positive or negative back-gate bias could keep the channel conductive or depleted throughout a limited top-gate sweep, showing why the biases must be coordinated.

![Top-gate transfer curves at different fixed back-gate voltages](figures/dual-gate-control.svg)

*V<sub>ds</sub> = 0.1 V; V<sub>bg</sub> from −50 to +50 V; V<sub>tg</sub> swept from −2 to +2 V. The corresponding top-gate current is shown alongside the transfer curves.*

### Switching and sweep-history dependence

With V<sub>bg</sub> = 70 V, extending the top-gate sweep to −4 V allowed channel depletion. The forward-sweep endpoint current ratio reached approximately 3.2 × 10⁶ at V<sub>ds</sub> = 0.5 V. Gate-controlled switching was also observed at lower drain biases, with smaller conducting-state currents.

![Dual-gate switching at four drain biases](figures/dual-gate-switching.svg)

*V<sub>bg</sub> = 70 V; V<sub>tg</sub> swept from −4 to +1 V and back; V<sub>ds</sub> = 1, 10, 100 and 500 mV.*

A separate measurement at V<sub>ds</sub> = 0.1 V gave a hysteresis width of approximately 0.25 V at I<sub>d</sub> = 100 pA. The separation varied with the reference current. This quantifies sweep-history-dependent conduction in the BSTO/MoS₂ gate stack; polarization-related electrostatics and charge trapping are relevant to its physical interpretation.

![Hysteresis window extracted at a 100 pA drain-current criterion](figures/dual-gate-hysteresis.svg)

*V<sub>bg</sub> = 70 V; V<sub>ds</sub> = 0.1 V. Forward/reverse separation is extracted at the same drain current.*

## Research contribution

This work demonstrates assembly and operation of BSTO/MoS₂ dual-gated transistors and shows how gate architecture, contact behaviour and leakage influence the measured response. It developed my experience connecting fabrication choices with electrical data and interpreting low-current measurements using simultaneous gate-current monitoring.

**Report:** *Van der Waals Integration of Perovskite Ferroelectric Ba₀.₆Sr₀.₄TiO₃ with 2D MoS₂ for High-Performance Dual-Gate Field-Effect Transistors* (NTU FYP, 2026).

**Related work:** [SJTU silicon photonics, graphene heaters and microring experiments](https://github.com/m220115-prog/NTU-SJTU-SILICON-PHOTONICS-2D-MODULATOR).

