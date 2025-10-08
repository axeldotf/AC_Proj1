# ⚡ Project 1 - Operational Amplifier Design

### **Author:** Alessandro Frullo  
*University of Bologna - Analog Circuits Op-Amp Project*

---

<p align="center">
  <a href="Project1_Frullo_v2.ipynb">
    <img src="https://img.shields.io/badge/Open%20Notebook-Project1_Frullo_v2.ipynb-blue?logo=jupyter&style=for-the-badge" alt="Open Notebook">
  </a>
</p>

<p align="center">
  <a href="Project1_Frullo_v2.pdf">
    <img src="https://img.shields.io/badge/View%20Report-Project1_Frullo_v2.pdf-red?logo=adobeacrobatreader&style=for-the-badge" alt="View PDF">
  </a>
</p>

<p align="center">
  <a href="https://drive.google.com/open?id=1gI2UxSNUznHZXjGs8nhtysiV_MXv-rLu&usp=drive_fs" target="_blank">
    <img src="https://img.shields.io/badge/Open%20Project%20Folder-Google%20Drive-green?logo=googledrive&style=for-the-badge" alt="Drive Folder">
  </a>
</p>

> ⚠️ **Acknowledgment**
> 
> The author used *ChatGPT (OpenAI, GPT-5)* as a tool to support text editing, data analysis, and documentation generation.  
> The final interpretation, validation, and presentation remain the author's sole responsibility.

---

## 🧾 Overview

This project focuses on the **design and sizing of a two-stage CMOS operational amplifier**.  
Starting from given **electrical specifications** and **technological parameters**, all transistor dimensions, biasing resistors, compensation elements, and small-signal parameters are derived analytically and verified through simulation.

The work includes:
- Analytical derivation of key design parameters (slew-rate, gain-bandwidth, noise).  
- Step-by-step **transistor sizing** and **current mirror balancing**.  
- Calculation of **compensation capacitance**, **biasing**, and **zero-nulling resistor**.  
- Verification of **DC gain**, **phase margin**, **power dissipation**, and **poles/zeros**.  
- SPICE-based validation of ICMR, output range, and frequency response.

---

## ⚙️ Project Specifications

| Parameter | Symbol | Value | Unit |
|:-----------|:-------:|:-------:|:------:|
| Supply voltages | VDD / VSS | +2.5 / −2.5 | V |
| Slew Rate | SR | ±5 | V/µs |
| Load Capacitance | CL | 5 | pF |
| Common-mode input voltage (max/min) | Vin,CM (max/min) | +2.1 / −1.3 | V |
| Output swing (max/min) | Vout (max/min) | +2.2 / −2.2 | V |
| Gain Bandwidth | GBW | 5 | MHz |
| Differential Gain | Ad | > 80 | dB |
| Phase Margin | PM | > 60 | ° |
| Equivalent Noise Density | Sn(f) | 30 | nV/√Hz (max) |

---

All computed **DataFrames** are exported automatically to `output_proj1_v2.xlsx`.

---

## 🧩 Requirements
```bash
pip install numpy pandas openpyxl
