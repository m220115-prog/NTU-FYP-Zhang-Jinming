# NTU-FYP-Zhang-Jinming
High-k 2D Dielectric Integration &amp; Leakage Current Suppression in2D FETs

## Fabrication & Characterization Workflow

The fabrication of these 2D heterostructure devices is a high-precision, multi-step process. Below is the detailed experimental workflow, highlighting the transfer mechanics, process optimization, and troubleshooting of real-world microfabrication challenges.

---

### 1. Material Preparation & Exfoliation

To prepare the 2D channels and dielectric layers, three distinct preparation and transfer strategies were employed:

*   **Mica Dielectric**: Few-layer Mica was mechanically cleaved from bulk crystals using adhesive tape and transferred onto transparent **PDMS stamps**.

<img width="2448" height="1920" alt="Mica" src="https://github.com/user-attachments/assets/b186c625-bf0b-4b64-8a71-b2dedb4f5b11" />

---

*   **BSTO Dielectric**: Ultrathin BSTO flakes were exfoliated and transferred onto **PDMS stamps** to act as high-k ferroelectric dielectric layers.

<img width="2448" height="1920" alt="BSTO" src="https://github.com/user-attachments/assets/b0fed329-c3bc-4940-b1d0-2f464c88bbdc" />

---

*   **MoS₂ Semiconductor**: Monolayer/few-layer MoS₂ was synthesized via **CVD**. To harvest the film, water-assisted transfer (utilizing water surface tension) was used to delaminate the MoS₂ from the growth substrate and place it onto **PDMS stamps**.

<img width="2448" height="1920" alt="MoS2" src="https://github.com/user-attachments/assets/91122764-58eb-4382-b444-9f05d2cb36ad" />

---

### Step 2: Van der Waals Stacking & Dry Transfer

Using a home-built high-precision transfer system, the 2D heterostructures were assembled via dry van der Waals integration:

*   **Precision Alignment**: Under an optical microscope, the target PDMS stamp (carrying MoS₂ or BSTO) was aligned with sub-micron precision over the substrate or pre-patterned electrodes.
*   **Mechanical Pressing & Adhesion**: Physical contact was made by slowly lowering the stamp. To overcome cases where the flake failed to adhere to the target surface, a localized thermal assistance (**heating the stage to ~60°C**) was applied to optimize the viscoelastic properties of PDMS, ensuring a clean and complete transfer.

| Transfer Equipment Setup | Precision Micro-Alignment & PDMS Release Process |
| :---: | :---: |
| <img width="480" height="600" alt="transferring equipment" src="https://github.com/user-attachments/assets/fae6345c-40b2-4c4a-bf95-f35be39de802" /> | <img width="480" height="600" alt="Transferring" src="https://github.com/user-attachments/assets/eb2300d8-53e9-49a6-a871-ae3ece148892" /> |

After the stacking steps, the intermediate states for the three main devices were successfully obtained:

| 1. Mica Back-Gate | 2. BSTO Back-Gate | 3. BSTO Top-Gate |
| :---: | :---: | :---: |
| <img width="2448" height="1920" alt="micabackgate" src="https://github.com/user-attachments/assets/c9f6ff90-cc2b-4b43-8b1e-ccd1a162f6f4" /> | <img width="2448" height="1920" alt="BSTObackgate" src="https://github.com/user-attachments/assets/eca638ed-f356-43ab-9339-51b1bf0129b7" /> | <img width="1920" height="2448" alt="BSTOtopgate" src="https://github.com/user-attachments/assets/ca5f9c71-c800-4358-8541-cbbc86761f08" /> |

---

### Step 3: Electrode Deposition & Fabrication Troubleshooting

Electrodes were patterned and deposited using **Electron-Beam Evaporation (EBL/E-beam evaporation)** with a **Cr/Au (5nm / 50nm)** metal stack. 

#### Process Troubleshooting: Electrode Peeling/Lift-off Failure
During early fabrication runs, we encountered a critical failure where **the deposited metal electrodes peeled off completely during the lift-off process**. 

*   **Root Cause Analysis**: 
    1.  **Electrode Dimensions**: The electrode fingers were designed too fine/narrow, leading to extremely poor aspect ratios and weak physical adhesion to the 2D channel/substrate.
    2.  **Environmental Factors**: High ambient humidity and continuous rainy days compromised the photoresist adhesion and introduced moisture interfaces.
    3.  **Target Materials**: Potential contamination or oxidation of the newly-supplied Cr/Au source material charges.
*   **The Solution**: We optimized the photolithography/EBL mask design by **increasing the width of the electrode lines (widening the contact pads and channels)** to enhance the contact area. This dramatically improved the mechanical adhesion of the metal film, yielding a 100% lift-off success rate in subsequent runs.

| 1. Fabricated Mica Back-Gate | 2. Fabricated BSTO Back-Gate | 3. Fabricated BSTO Top-Gate |
| :---: | :---: | :---: |
| <img width="2448" height="1920" alt="mica E" src="https://github.com/user-attachments/assets/2ea993a4-be38-4794-967a-95aafa971b21" /> | <img width="2448" height="1920" alt="BSTO E2" src="https://github.com/user-attachments/assets/d7114711-4985-4d71-8288-54ddb549abcd" /> | <img width="2448" height="1920" alt="BSTO top E" src="https://github.com/user-attachments/assets/84f49cad-c599-4a9b-bfe4-a6521fb40b80" /> |

---

### Step 4: Electrical Probing & Device Characterization

To verify the structural and physical integrity of the devices, they were first inspected under **Optical Microscopy** and **Scanning Electron Microscopy (SEM)**. 

Systematic electrical characterization was then performed at room temperature inside a **shielded probe station** using a **Keysight B1500A Semiconductor Parameter Analyzer**.

#### Case Study: Double-Gate Modulation & Memory Window in BSTO Top-Gate
The high-performance **BSTO Top-Gate FET** features a unique double-gate configuration (utilizing both the silicon back-gate and the BSTO top-gate). This device provided our most comprehensive and authoritative dataset:

1.  **N-type Transistor Behavior**: Confirmed robust n-channel transport characteristics in the MoS₂ channel, showing an excellent On/Off current ratio.
2.  **Ferroelectric Memory Window**: The double-sweep hysteresis curves demonstrate a stable **0.8V memory window** under top-gate voltage modulation, proving the non-volatile polarization switching of the integrated BSTO layer.
3.  **Gate-Control Comparison (Successful vs. Leaky Back-Gate)**: 
    *   *Our Top-Gate device* showed pristine switching.
    *   *Comparison with Failed/Leaky Devices*: To highlight the critical role of gate dielectric optimization, we plot our successful curves alongside data from a **failed/leaky back-gate device** (which suffered from high gate leakage current $I_g$). This comparison clearly demonstrates how the top-gate BSTO integration successfully suppresses leakage current and restores gate control.

<!-- 💡 upload: top_gate_hysteresis.png & leaky_vs_good_comparison.png -->
| Top-Gate Dual-Sweep Hysteresis (0.8V Window) | Leakage Suppression Comparison (Good vs. Leaky Device) |
| :---: | :---: |
| ![Hysteresis Curve](images/top_gate_hysteresis.png) | ![Leaky vs Good](images/leaky_vs_good_comparison.png) |
















