## FinFET Circuit Design and Characterization
This GitHub repository documents the 10-day workshop on FinFET Circuit Design and Characterization using ASAP7 PDK offered by VSD Corp. Pvt. Ltd. attended from 27 Aug - 05 Sept, 2025.

Table of Contents

| Module # | Topic(s) Covered |
 |---|---|
 |[**Mod. 1**](#1---scaling-beyond-cmos-finfet-devices-and-innovations) | **Scaling Beyond CMOS: FinFET Devices and Innovations** <br> <ol> <li>[Path To Zetta Scale Computing](#11---path-to-zetta-scale-computing)</li> <li>[Introduction To FinFETs](#12---introduction-to-finfets)</li> <li>[FEOL Innovations](#13-feol-innovations)</li> <li>[BEOL Innovations](#14---beol-innovations)</li> </ol> |
 |[**Mod. 2**](#2---lab-to-simulation-7nm-finfet-inverter-performance-analysis) | **Lab-to-Simulation: 7nm FinFET Inverter Performance Analysis** <br> <ol> <li>[NFET DC Characteristics Using 7nm PDKs](#21---nfet-dc-characteristics-using-7nm-pdks)</li> <li>[First Inverter Characteristics Using 7nm FinFETs](#22---first-inverter-characteristics-using-7nm-finfets)</li><li>[Module 2 Assignment - 7nm Inverter Characterization](#23---module-2-assignment---7nm-inverter-characterization)</li> </ol> |
 |[**Mod. 3**](#3---design-of-a-bandgap-reference-circuit) | **Design of a BandGap Reference Circuit** <br> <ol> <li>[Theory: Design of a BGR Circuit](#31---theory-design-of-a-bgr-circuit)</li> <li>[Module 3 Assignent - Bandgap Reference Design and Simulation using Xschem](#32---module-3-assignent---bandgap-reference-design-and-simulation-using-xschem)</li> </ol> |
 
## 1.1 - Scaling Beyond CMOS: FinFET Devices and Innovations

---

  Path to Zetta-Scale Computing
- **FinFETs**
- **FEOL Innovations**
- **BEOL Innovations**

---

  Problems to Solve
  In the Beginning
- **Bombe** – Break Enigma code; Mechanical and Application-Specific
- **ENIAC** – Vacuum tubes, Decimal Number System, Turing-based
- **EDVAC** – Vacuum tubes, Binary Number System, complete Von Neumann Architecture
- **CMOS** – Implementation of ENIAC using CMOS technology

---

  Next Generation Computing Goals
- Validate **Fundamental laws of Nature**
- Develop **Next-generation Semiconductors**
- **Weather Modeling and Forecasting**
- **Health and Precision Medicine**
- **Virtual Particle Accelerators**
- **Room-temperature Superconductors**
- **Earthquake Modeling**
- **Earth–water Cycle Analysis**

---

  FLOPs
- **FLOPs** = Floating Point Operations Per Second

  Unit Scale (for Compute)
- **Giga → Tera → Peta → Exa → Zetta**

---

## 1.2 CMOS Evolution and Next-Gen Candidates

<img width="792" height="438" alt="Mod1_lecture_02" src="https://github.com/user-attachments/assets/015879e9-766e-433d-ad4d-aea7e7e40947" />

---

## 1.3 Introduction To FinFETs

FinFET stands for Fin Field Effect Transistor it belongs to the FET family and it is a type of Multi gate MOSFET that is used in place of a common MOSFET.

Key Features of FinFET Technology
3D Structure: The vertical fin design improves control over the channel, allowing for higher performance at smaller nodes.
Improved Electrostatic Control: By surrounding the channel with the gate on three sides, FinFETs reduce leakage currents and improve switching speeds.
Scalability: FinFET technology enables continued scaling of transistors beyond the limitations faced by planar designs.

<img width="2352" height="1217" alt="Screenshot 2025-09-16 003643 - Copy" src="https://github.com/user-attachments/assets/549e4e57-213f-4fe7-943d-8151e4ea0c7d" />

Why FinFets?

To follow Moore’s, we have to increase the number of transistors which leads to downscaling of the transistor dimensions and results in several SCEs.
FinFET is one of the favorable devices due to more controllability of the gate over the channel
Chenming Hu, and his group in 1998 were the first who coined the term FinFET, as a result of the structure.

<img width="2339" height="1256" alt="Screenshot 2025-09-16 004019" src="https://github.com/user-attachments/assets/59125d12-2e20-478c-af98-f912481a28a4" />

---
## 1.4 CMOS Technology Inflection Points

<img width="2213" height="1066" alt="Screenshot 2025-09-16 004724" src="https://github.com/user-attachments/assets/190071a9-e008-489e-9967-8e6e2a929313" />

<img width="2329" height="1107" alt="Screenshot 2025-09-16 005348" src="https://github.com/user-attachments/assets/c809e383-3e5d-4c3f-9b02-1d0dcdf70cb3" />

---

## 1.5 Standard Cell Area Scaling: Fin Depopulation

<img width="2106" height="928" alt="Screenshot 2025-09-16 005808" src="https://github.com/user-attachments/assets/75151f8f-2e66-40f6-88d8-23b68f55ca45" />

Standard Cell Area Scaling :- SDB, COAG, BS-PDN

<img width="2220" height="1068" alt="Screenshot 2025-09-16 005900" src="https://github.com/user-attachments/assets/07e21ace-48e6-4dbc-91de-d70558c31983" />

---

## 1.6 Parasitic Resistance

<img width="2189" height="699" alt="Screenshot 2025-09-16 010801" src="https://github.com/user-attachments/assets/f325ac8b-b532-4fc3-86df-902f80ddd3f3" />

<img width="2262" height="941" alt="Screenshot 2025-09-16 011340" src="https://github.com/user-attachments/assets/53e30135-8b54-4660-9654-554a7e31064f" />

---

## 1.7 Device Scaling Using Layered Materials

Important material properties relative to silicon
- ** a) Uniform atomic scale thickness (thickness scaling limit (~0.65nm MoS₂ monolayer) 
- ** b) Effective mass m* higher (~0.55 mo for MoS₂ compared to ~0.22 mo for silicon)  
- ** c) Bandgap (eg MoS₂ monolayer ~1.85ev, MoS₂ bilayer ~1.5ev)

<img width="1259" height="666" alt="Screenshot 2025-09-16 012833" src="https://github.com/user-attachments/assets/14bcb6e3-9738-4223-9732-e5076d6e4b57" />

---

Transistor Scaling to sub-5nm Gate Lengths

Transistor scaling for higher packing density, better performance, lower cost.

Challenges for scaling

- ** a) Direct source-to-drain tunneling leakage, need high effective mass (m*).
- ** b) Surface roughness and thickness variations, uniform atomically thin materials.
- ** c) CD high relative to Cox, need low-in plane dielectric constant (ε) and new channel material.
  
---

Direct Source-to_Drain Tunneling

- * Up to 100x reduction in direct source to drain tunneling leakage due to higher m*, Larger Eg and lower ε of MoS₂ relative to silicon.
- * Large energy savings in electronics.
 
<img width="2358" height="985" alt="Screenshot 2025-09-16 013236" src="https://github.com/user-attachments/assets/35891953-0ea0-4f38-b35f-39cf682bf439" />

---

 MoS₂ Transistor with 1nm Gate Length

- * 1nm single walled carbon nanotube gate with MoS₂ channel.
- * Shortest gate length transistor demonstarted.
- * MoS₂ extensions inverted using gloabl si back gate and CNT gate depletes a small region of MoS₂ above it.
- * Large energy savings in electronics.
    
---



