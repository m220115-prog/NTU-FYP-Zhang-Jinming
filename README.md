<img width="2448" height="1920" alt="image" src="https://github.com/user-attachments/assets/c11cabb1-fff6-48dd-b09b-54a10971b36a" /># NTU-FYP-Zhang-Jinming
High-k 2D Dielectric Integration &amp; Leakage Current Suppression in2D FETs

Welcome! This repository documents my Final Year Project at Nanyang Technological University (NTU), focusing on the design, fabrication, and characterization of novel 2D material-based Field-Effect Transistors (FETs).

The core of this project is to address the performance bottlenecks of 2D material FETs by integrating novel high-k dielectric materials. I successfully fabricated and compared three types of devices: **Mica back-gate**, **BSTO back-gate**, and a high-performance **BSTO top-gate** structure.

---

## 🔬 Fabrication & Characterization Workflow

The fabrication process is a multi-step procedure involving material preparation, precision transfer, and electrode deposition. Here is a visual overview of the key steps.

*   **Step 1: Material Preparation** -> **Step 2: Van der Waals Stacking** -> **Step 3: Electrode Deposition** -> **Step 4: Electrical Probing**
*  <img width="2448" height="1920" alt="1-50" src="https://github.com/user-attachments/assets/e3a08922-976e-4252-8d5a-82c2f504be2e" />



**(💡 操作提示：请在这里上传您提到的“最初材料”、“转移好的”、“镀电极的”和“测试”的照片，并修改下面的文件名)**

| Material (MoS₂, BSTO, Mica) | Precision Transfer | Electrode Deposition | Probing & Measurement |
| :---: | :---: | :---: | :---: |
| ![Material Preparation](initial_materials.png) | ![Device Transfer](transfer_process.png) | ![Electrode Deposition](electrode_deposition.png) | ![Device Testing](testing_setup.png) |

---

## 🏆 Key Result: Top-Gate BSTO/MoS₂ Ferroelectric Transistor

The highlight of this project is the successful fabrication of a top-gate FET using a **Barium Strontium Titanate (BSTO)** ferroelectric dielectric. This device not only demonstrates superior transistor performance but also exhibits non-volatile memory capabilities.

### 1. Non-Volatile Memory Effect (Hysteresis Loop)

The dual-sweep transfer curve ($I_d-V_g$) below clearly shows a large, stable memory window of **~0.8V**. This is direct evidence of ferroelectric polarization switching in the BSTO layer, enabling the device to store information without power. This is the key advantage over conventional Mica or standard BSTO back-gate structures.

**(💡 操作提示：请上传您挑选出的 `IdVd-Vt-dual [8]...png` 文件，并将其重命名为 `top_gate_hysteresis.png` 后放在这里)**

![Transfer Curve with Hysteresis](top_gate_hysteresis.png)

### 2. Excellent Transistor Output Characteristics

The output characteristics ($I_d-V_d$) confirm the device's robust transistor behavior. The curves show clear saturation regions and excellent gate modulation, indicating high-quality channel and contact.

**(💡 操作提示：请上传您挑选出的 `IdVd-Vd-dual [10]...png` 文件，并将其重命名为 `top_gate_output.png` 后放在这里)**

![Output Characteristics](top_gate_output.png)

---

## 📊 Device Comparison & Summary

| Device Structure | Dielectric Material | Key Feature | Performance Summary |
|:---|:---|:---|:---|
| **BSTO Top-Gate** | **BSTO (Ferroelectric)** | **Non-Volatile Memory** | **Excellent!** Achieved >10⁵ On/Off ratio and a stable 0.8V memory window. |
| BSTO Back-Gate | BSTO (High-k) | High-k Advantage | **Good.** Showed significantly improved gate control (SS ≈ 110 mV/dec) compared to Mica. |
| Mica Back-Gate | Mica (Conventional) | Baseline/Control | **Fair.** Acted as a baseline, suffered from higher subthreshold swing and interface defects. |
