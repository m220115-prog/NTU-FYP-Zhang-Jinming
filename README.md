# NTU-FYP-Zhang-Jinming
High-k 2D Dielectric Integration & Leakage Current Suppression in 2D FETs

## Fabrication & Characterization Workflow

Fabricating these 2D heterostructures requires precise micro-manipulation. Here is my hands-on fabrication process, where I resolved the electrode adhesion issues and processed all the electrical test data.

---

### Step 1: Material Preparation & Exfoliation

Preparing the 2D channels and dielectric layers involved three distinct exfoliation and transfer strategies:

* **Mica Dielectric:** Few-layer Mica was mechanically cleaved from bulk crystals using adhesive tape and transferred onto transparent PDMS stamps.
<img width="2448" height="1920" alt="Mica" src="https://github.com/user-attachments/assets/b186c625-bf0b-4b64-8a71-b2dedb4f5b11" />

* **BSTO Dielectric:** Ultrathin BSTO flakes were exfoliated and transferred onto PDMS stamps to serve as high-k ferroelectric dielectric layers.
<img width="2448" height="1920" alt="BSTO" src="https://github.com/user-attachments/assets/b0fed329-c3bc-4940-b1d0-2f464c88bbdc" />

* **MoS₂ Semiconductor:** Monolayer/few-layer MoS₂ was synthesized via CVD. To harvest the film, water-assisted transfer (utilizing water surface tension) was used to delaminate the MoS₂ from the growth substrate and place it onto PDMS stamps.
<img width="2448" height="1920" alt="MoS2" src="https://github.com/user-attachments/assets/91122764-58eb-4382-b444-9f05d2cb36ad" />

---

### Step 2: Van der Waals Stacking & Dry Transfer

Dry van der Waals integration was carried out using a home-built high-precision transfer system to assemble the 2D heterostructures:

* **Precision Alignment:** Under an optical microscope, the target PDMS stamp (carrying MoS₂ or BSTO) was aligned with sub-micron precision over the substrate or pre-patterned electrodes.
* **Mechanical Pressing & Adhesion:** Physical contact was made by slowly lowering the stamp. In cases where the flakes failed to adhere to the target surface, heating the stage to ~60°C optimized the viscoelastic properties of PDMS, ensuring a clean and complete transfer.

| Transfer Equipment Setup | Precision Micro-Alignment & PDMS Release Process |
| :---: | :---: |
| <img width="400" height="500" alt="transferring equipment" src="https://github.com/user-attachments/assets/16878f50-e6ad-4c73-8bc6-216d812f8a99" /> | <img width="400" height="500" alt="transfer" src="https://github.com/user-attachments/assets/97605128-49e4-49e3-a28f-3aebbdc53d74" /> |

After the stacking steps, the intermediate states for the three main devices were successfully obtained:

| 1. Mica Back-Gate | 2. BSTO Back-Gate | 3. BSTO Top-Gate |
| :---: | :---: | :---: |
| <img width="2448" height="1920" alt="micabackgate" src="https://github.com/user-attachments/assets/c9f6ff90-cc2b-4b43-8b1e-ccd1a162f6f4" /> | <img width="2448" height="1920" alt="BSTObackgate" src="https://github.com/user-attachments/assets/eca638ed-f356-43ab-9339-51b1bf0129b7" /> | <img width="2448" height="1920" alt="BSTOtopgate" src="https://github.com/user-attachments/assets/7e96b135-a4ba-434b-a792-e3dfe4c9603a" /> |

---

### Step 3: Electrode Deposition & Fabrication Troubleshooting

Source/drain electrodes were patterned via Electron-Beam Lithography (EBL) and deposited with a Cr/Au (5nm / 50nm) metal stack using E-beam evaporation.

#### Process Troubleshooting: Electrode Peeling and Lift-off Failure

During early fabrication runs, a critical failure occurred where the deposited metal electrodes peeled off completely during the lift-off process. 

| Electrode Peeling (Failure Case) | Widened Electrodes (Optimized & Resolved) |
| :---: | :---: |
| <img width="2448" height="1920" alt="BSTO E1" src="https://github.com/user-attachments/assets/40400440-7289-4ff6-ad4a-39d13bd6ace2" /> | <img width="2448" height="1920" alt="BSTO E2" src="https://github.com/user-attachments/assets/23aa55f1-d232-44b9-9d29-fe9491c65f10" /> |

**Root Cause Analysis:** 
1. **Electrode Dimensions:** The electrode fingers were initially designed too narrow, leading to extremely poor aspect ratios and weak physical adhesion to the 2D channel and substrate.
2. **Environmental Factors:** High ambient humidity during continuous rainy days compromised the photoresist adhesion and introduced moisture interfaces.

**The Solution:** Optimizing the EBL mask design by increasing the width of the electrode lines (widening the contact pads and channels) enhanced the contact area. This modification significantly improved the mechanical adhesion of the metal film, yielding a 100% lift-off success rate in subsequent runs.

| 1. Fabricated Mica Back-Gate | 2. Fabricated BSTO Back-Gate | 3. Fabricated BSTO Top-Gate |
| :---: | :---: | :---: |
| <img width="2448" height="1920" alt="mica E" src="https://github.com/user-attachments/assets/2ea993a4-be38-4794-967a-95aafa971b21" /> | <img width="2448" height="1920" alt="BSTO E3" src="https://github.com/user-attachments/assets/0dfd1178-8f97-45e5-bc61-277325b3bbe8" /> | <img width="2448" height="1920" alt="BSTO top E" src="https://github.com/user-attachments/assets/84f49cad-c599-4a9b-bfe4-a6521fb40b80" /> |

---

### Step 4: Electrical Probing & Device Characterization

Confirming the structural and physical integrity of the devices started with inspections under Optical Microscopy and Scanning Electron Microscopy (SEM). Systematic electrical characterization was then performed at room temperature inside a shielded probe station using a Keysight B1500A Semiconductor Parameter Analyzer.

#### 4.1 Output Characteristics & N-type Conduction

Output characteristics (Id-Vd) were measured by sweeping the drain voltage (Vd) while stepping the back-gate voltage (Vg) from -50V to 50V. The resulting curves confirm proper field-effect transistor operation. The drain current (Id) systematically increases with more positive back-gate bias, providing definitive evidence of **n-type (electron-dominated) carrier transport** in the MoS₂ channel. Furthermore, the linear (ohmic) behavior at low Vd and clear current saturation at high Vd indicate good ohmic contacts and pinch-off behavior.

<img width="881" height="356" alt="IdVd-Vb-dual" src="https://github.com/user-attachments/assets/f4487fdc-e122-44e8-a4bd-7d9bc7185b15" />

---

#### 4.2 Dual-Gate Tunability of Threshold Voltage

To demonstrate dual-gate control, transfer characteristics (Id-Vtg) were evaluated by sweeping the top-gate voltage (Vtg) under various fixed back-gate biases (Vbg from -50V to 50V). The parallel shift of the transfer curves to the left with increasing positive Vbg provides clear evidence of **threshold voltage tunability**. This behavior is characteristic of a dual-gate FET, where the back-gate acts as a secondary control terminal, effectively modulating the electrostatic environment of the MoS₂ channel and allowing for reconfigurable device performance.

<img width="881" height="356" alt="IdVt-dual 1" src="https://github.com/user-attachments/assets/b93915cf-3be4-4544-9bec-d2f0c351b571" />

---

#### 4.3 Non-Volatile Memory from Ferroelectric Top-Gate

The core innovation of this device is the non-volatile memory effect, verified by a dual-sweep measurement of the top-gate transfer curve (Id-Vtg) from -4V to 1V and back. The resulting counter-clockwise **hysteresis loop**, with a clear memory window, is direct proof of ferroelectric polarization switching in the BSTO dielectric. This switching persistently modulates the MoS₂ channel's resistance state even at zero gate bias, confirming the device's function as a non-volatile memory element (FeFET).

<img width="881" height="356" alt="IdVt-dual 5" src="https://github.com/user-attachments/assets/ef357446-f5d6-476f-8c2c-1f18e8ec4a36" />

---

#### 4.4 Architecture Benchmarking: Top-Gate vs. Failed Back-Gate

A key motivation for developing the top-gate architecture was to overcome the significant challenges associated with back-gate configurations for these materials, namely poor interface quality and dielectric breakdown. Benchmarking the optimized top-gate design against two representative failed BSTO back-gate devices highlights these structural advantages.

The back-gate devices exhibited two distinct, critical failure modes:

1. **Loss of Gate Control (Left):** The device shows no switching behavior (On/Off ratio ≈ 1). The gate electric field is completely screened, likely due to an extremely high density of interface traps between the BSTO and the MoS₂ channel, rendering the device non-functional.
2. **High Gate Leakage (Middle):** The gate leakage current (Ig, orange curve) is on the same order of magnitude as the drain current (Id, blue curve). This indicates a catastrophic breakdown of the BSTO dielectric, where current leaks directly through the gate instead of modulating the channel.

In stark contrast, the optimized top-gate architecture (Right) effectively suppresses both interface traps and leakage current. This integration results in a clean, stable, and large hysteresis loop, confirming its robust performance.

| Failure Mode 1: No Switching | Failure Mode 2: High Gate Leakage | Success: Optimized Top-Gate |
| :---: | :---: | :---: |
| <img width="881" height="356" alt="No Switching" src="https://github.com/user-attachments/assets/8507cc9c-3a14-4d73-903c-b694bfb49b7e" /> | <img width="881" height="356" alt="Leakage" src="https://github.com/user-attachments/assets/05015d51-8937-4532-a04a-71bb94beb10a" /> | <img width="881" height="356" alt="Success" src="https://github.com/user-attachments/assets/ef357446-f5d6-476f-8c2c-1f18e8ec4a36" /> |
