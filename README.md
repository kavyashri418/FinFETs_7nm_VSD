FinFET Circuit Design and Characterization
This GitHub repository documents the 10-day workshop on FinFET Circuit Design and Characterization using ASAP7 PDK offered by VSD Corp. Pvt. Ltd. attended from 27 Aug - 05 Sept, 2025.

Table of Contents

| Module # | Topic(s) Covered |
 |---|---|
 |[**Mod. 1**](#1---scaling-beyond-cmos-finfet-devices-and-innovations) | **Scaling Beyond CMOS: FinFET Devices and Innovations** <br> <ol> <li>[Path To Zetta Scale Computing](#11---path-to-zetta-scale-computing)</li> <li>[Introduction To FinFETs](#12---introduction-to-finfets)</li> <li>[FEOL Innovations](#13-feol-innovations)</li> <li>[BEOL Innovations](#14---beol-innovations)</li> </ol> |
 |[**Mod. 2**](#2---lab-to-simulation-7nm-finfet-inverter-performance-analysis) | **Lab-to-Simulation: 7nm FinFET Inverter Performance Analysis** <br> <ol> <li>[NFET DC Characteristics Using 7nm PDKs](#21---nfet-dc-characteristics-using-7nm-pdks)</li> <li>[First Inverter Characteristics Using 7nm FinFETs](#22---first-inverter-characteristics-using-7nm-finfets)</li><li>[Module 2 Assignment - 7nm Inverter Characterization](#23---module-2-assignment---7nm-inverter-characterization)</li> </ol> |
 |[**Mod. 3**](#3---design-of-a-bandgap-reference-circuit) | **Design of a BandGap Reference Circuit** <br> <ol> <li>[Theory: Design of a BGR Circuit](#31---theory-design-of-a-bgr-circuit)</li> <li>[Module 3 Assignent - Bandgap Reference Design and Simulation using Xschem](#32---module-3-assignent---bandgap-reference-design-and-simulation-using-xschem)</li> </ol> |
 
# 1.1 - Scaling Beyond CMOS: FinFET Devices and Innovations

## Overview
This document explores the path to **Zetta-scale computing**, focusing on innovations in FinFET devices, FEOL (Front-End-Of-Line), and BEOL (Back-End-Of-Line) technologies.

---

## Path to Zetta-Scale Computing
- **FinFETs**
- **FEOL Innovations**
- **BEOL Innovations**

---

## Problems to Solve

### In the Beginning
- **Bombe** – Broke Enigma code; mechanical and application-specific
- **ENIAC** – Vacuum tubes, decimal number system, Turing-based
- **EDVAC** – Vacuum tubes, binary number system, complete Von Neumann architecture
- **CMOS** – Implementation of ENIAC using CMOS technology

---

## Next Generation Computing Goals
- Validate **fundamental laws of nature**
- Develop **next-generation semiconductors**
- **Weather modeling and forecasting**
- **Health and precision medicine**
- **Virtual particle accelerators**
- **Room-temperature superconductors**
- **Earthquake modeling**
- **Earth–water cycle analysis**

---

## Performance Metrics

### FLOPs
- **FLOPs** = Floating Point Operations Per Second

### Performance Targets
- **FP64 (Tensor)**  
  - **ZettaFLOP** = 10^21 FLOPs/second  
  - **Power Consumption:** 50–100 MW

- **FP32 (Tensor)**  
  - ZettaFLOP-level performance for single-precision workloads

- **BF16 / Int8 (Tensor)**  
  - Peak performance in the range of **8–16 ZettaFLOPs**

---

## Unit Scale (for Compute)
- **Giga → Tera → Peta → Exa → Zetta**

---

## Key Takeaways
Achieving ZettaFLOP-scale computing will require:
- Breakthroughs in semiconductor scaling (FinFETs and beyond)
- Innovations in FEOL & BEOL processing
- Efficient power management for massive performance targets
- New materials (e.g., room-temperature superconductors)
- Support for next-gen scientific workloads and global modeling challenges
  
# 1.2 CMOS Evolution and Next-Gen Candidates

This repository explores **CMOS evolution** and the **next-generation device candidates** required to scale semiconductor technology into the future.

---

## Overview

CMOS (Complementary Metal-Oxide Semiconductor) technology has been the backbone of modern electronics for decades. However, as we approach the limits of Moore's Law, innovations are required in multiple areas — **materials, device structures, patterning, and interconnects** — to keep advancing.

---

## Technology Evolution Roadmap

The diagram below represents the evolution path of CMOS technology and possible next-generation candidates:

### Patterning Innovations
- **High NA EUV**
- **EUV (Extreme Ultraviolet Lithography)**
- **QPT, DPT (Quad / Double Patterning Techniques)**
- **SAQP (Self-Aligned Quadruple Patterning)**

---

### Channel Materials
- **2D Materials**
- **SiGe (Silicon-Germanium)**

---

### Interconnect Material Innovations
- **Ru (Ruthenium)**
- **Cu (Copper)**
- **Topological Semimetals**

---

### Gate Stack Material
- **HKMG (High-k / Metal Gate)**
- **NC-FET (Negative Capacitance FET)**

---

### Device Structure Innovations
- **FinFET (Current Technology Node)**
- **GAAFET / MBC-FET (Gate-All-Around, Multi-Bridge Channel FET)**
- **TFET (Tunnel FET)**
- **VFET (Vertical FET)**
- **BDS-FET (Backside FET)**
- **DTCO (Design-Technology Co-Optimization)**

---

### System-Level Innovations
- **BS-PDN (Backside Power Delivery Network)**
- **STCO (System-Technology Co-Optimization)**
- **Chiplets** – Modular SoC integration for heterogeneous computing

---

## Timeline
- **Now:** FinFET-based nodes
- **Future:** GAAFET, MBC-FET, and advanced interconnect/material/device innovations leading to ultimate scaling near 1 nm technology nodes

---

## Key Takeaways
- Scaling requires **parallel innovation** in:
  - Patterning (lithography, multiple patterning)
  - Channel materials (new semiconductors, 2D materials)
  - Interconnect and gate stack materials
  - Device structures (FinFET → GAAFET → Beyond)
  - System-level co-optimization (BS-PDN, STCO, chiplets)

- The **combination of materials + design + architecture** will define the next era of semiconductor technology.

---

# 1.3 Introduction to FinFETs
https://github.com/kavyashri418/FinFETs_7nm_VSD/blob/main/WhatsApp%20Image%202025-09-23%20at%202.43.14%20PM%20(1).jpeg?raw=true
This repository provides a clear and concise introduction to **FinFET (Fin Field-Effect Transistor)** technology — the workhorse of modern semiconductor scaling — including its structure, advantages, and challenges.

---

## What is a FinFET?

A **FinFET** is a type of multi-gate transistor used in modern CMOS process nodes (22nm and below).  
Unlike planar MOSFETs, FinFETs have a **3D fin-like channel** that rises above the substrate, allowing the gate to wrap around the channel on three sides.

---

## Key Features

- **3D Structure**  
  - Channel is shaped like a fin  
  - Gate wraps around three sides of the channel

- **Better Electrostatic Control**  
  - Reduced short-channel effects  
  - Lower leakage current

- **Scalability**  
  - Enables continued Moore’s Law scaling below 22nm nodes

---

## Advantages of FinFETs

- ✅ **Lower Leakage Power** – Gate control reduces off-state leakage  
- ✅ **Better Performance** – Higher drive current, improved switching speed  
- ✅ **Energy Efficiency** – Lower operating voltage (Vdd)  
- ✅ **Density Scaling** – Smaller footprint compared to planar FETs

---

## Challenges

- ⚠️ **Complex Fabrication** – Requires advanced lithography and etching  
- ⚠️ **Higher Cost** – More expensive manufacturing process  
- ⚠️ **Parasitics** – Increased parasitic capacitances due to 3D structure  
- ⚠️ **Design Complexity** – Requires new EDA tools and design methodologies  

---

## Applications

- Used in **high-performance CPUs, GPUs, and SoCs**  
- Found in **mobile processors** (smartphones, tablets)  
- Deployed in **data center processors** for efficiency and performance  
- Critical for **AI accelerators** and **next-gen networking chips**

---

# Impact of FinFETs on Circuit Performance

This repository explains how **FinFET technology** improves circuit-level performance compared to planar CMOS transistors.  

---

## Overview

FinFETs offer **better electrostatic control**, lower leakage, and improved scalability, leading to significant **performance, power, and area (PPA)** benefits at the circuit level.

---

## Key Impacts on Circuit Performance

### 1. **Improved Drive Current (ION)**
- Higher effective channel width (due to vertical fins)
- Increased drive current per unit footprint
- Faster switching speeds → **higher operating frequency**

---

### 2. **Reduced Leakage Current (IOFF)**
- Stronger gate control reduces subthreshold leakage
- Significant reduction in standby power
- Enables **low-power circuit design**

---

### 3. **Lower Supply Voltage (VDD)**
- FinFETs can operate at lower VDD without sacrificing performance
- Leads to **dynamic power reduction** (P ∝ VDD²)

---

### 4. **Better Short-Channel Control**
- Reduced DIBL (Drain-Induced Barrier Lowering)
- Lower variability → more reliable circuits at smaller nodes

---

### 5. **Higher Frequency Operation**
- Faster switching → higher maximum clock frequency
- Benefits **high-performance computing (HPC)** and **AI accelerators**

---

### 6. **Area Efficiency**
- Multi-fin devices can achieve desired drive strength in smaller footprint
- Higher integration density → more logic per mm²

---

### 7. **Impact on Analog/RF Circuits**
- Better gm/Id ratio → improved transconductance efficiency
- Lower parasitic capacitances → higher cutoff frequency (fT)
- Enables **low-power, high-speed analog and RF designs**

---

## Trade-Offs and Challenges

- **Parasitic Capacitance:** Increased overlap capacitance may impact very high-speed designs  
- **Design Complexity:** Requires multi-fin sizing and discrete width quantization  
- **EDA Tool Support:** Demands updated SPICE models and physical design flows  
- **Variability:** Fin height/width variation can affect matching in analog circuits  

---

# 1.3 CMOS Technology Inflection Points

This repository documents **key inflection points in CMOS technology** — the major innovations that have enabled continued scaling of transistors over decades.  

---

## Introduction

CMOS (Complementary Metal-Oxide Semiconductor) technology has driven the semiconductor industry for more than 50 years.  
However, to keep up with **Moore's Law**, the industry has had to introduce **new materials, device structures, and patterning techniques** at critical inflection points.

---

## Key Inflection Points

### 1. **Planar CMOS Era**
- **Channel:** Silicon (Bulk)  
- **Gate Dielectric:** SiO₂  
- **Node Range:** > 90nm  
- **Challenges:** Short-channel effects, leakage power

---

### 2. **High-k / Metal Gate (HKMG) Introduction**
- **Key Node:** ~45nm  
- **Innovation:** Replaced SiO₂ with High-k dielectric (e.g., HfO₂) and poly-Si gate with metal gate  
- **Benefit:** Reduced gate leakage, improved electrostatic control

---

### 3. **Stress Engineering & Strained Silicon**
- **Node Range:** 90nm → 32nm  
- **Innovation:** Strain in the channel increases carrier mobility  
- **Benefit:** Boosts drive current and performance

---

### 4. **FinFET / Tri-Gate Transistor Era**
- **Key Node:** ~22nm (Intel’s 3D Tri-Gate)  
- **Innovation:** 3D fin structure with gate wrapping around the channel  
- **Benefit:** Lower leakage, better short-channel control, scalability below 20nm

---

### 5. **EUV Lithography Adoption**
- **Node Range:** 7nm → 5nm → 3nm  
- **Innovation:** Extreme Ultraviolet Lithography (EUV) for finer patterning  
- **Benefit:** Simplifies multi-patterning, improves yield

---

### 6. **GAAFET / MBCFET Introduction (Future)**
- **Node Range:** < 3nm  
- **Innovation:** Gate-All-Around architecture (nanosheet or nanowire FET)  
- **Benefit:** Superior electrostatic control, improved performance-per-watt

---

### 7. **System-Technology Co-Optimization (STCO) & Chiplets**
- **Current Trend:** Heterogeneous integration, 3D packaging, chiplet-based SoCs  
- **Focus:** Power delivery (BS-PDN), interconnect scaling, 3D-IC stacking  
- **Benefit:** Performance scaling beyond transistor-level scaling

---

# 1.4 - Standard Cell Area Scaling & Fin Depopulation

This repository explains **Standard Cell Area Scaling** techniques, with a focus on **Fin Depopulation** — a critical strategy used in advanced process nodes to reduce area while balancing performance, power, and yield.

---

## What is Standard Cell Area Scaling?

A **standard cell** is the fundamental building block of a digital integrated circuit.  
**Standard cell area scaling** is the process of reducing the footprint of these cells to pack more logic per mm², improving density, performance, and cost efficiency.

---

## Fin Depopulation – Key Concept

**Fin Depopulation** refers to reducing the **number of fins per transistor** in a standard cell while still meeting performance targets.

### Example:
- At larger nodes: **4 fins per transistor** (high drive strength, more area)
- At advanced nodes: **2 or 3 fins per transistor** (optimized density, lower power)

This technique is crucial in **area-optimized libraries**.

---

## Benefits of Fin Depopulation

- ✅ **Smaller Standard Cell Height** – Improves logic density  
- ✅ **Lower Power Consumption** – Fewer fins → lower drive current → less switching power  
- ✅ **Better Cost Efficiency** – More transistors per wafer  
- ✅ **Supports Multi-Vt Options** – Can offer HP (high-performance), HD (high-density) cell libraries

---

## Challenges

- ⚠️ **Performance Loss** – Fewer fins reduce drive strength  
- ⚠️ **Increased Variability** – Device mismatch and process variation impact timing  
- ⚠️ **Routing Congestion** – Tighter pitches make routing difficult  
- ⚠️ **EDA Complexity** – Requires re-optimized PDK and cell libraries

---

## Techniques for Area Scaling

- **Track Height Reduction**  
  - Example: 9T → 7.5T → 6T libraries (tracks refer to metal routing tracks per cell)
- **Contact Over Active Gate (COAG)**  
  - Reduce cell height by placing contacts directly over gate
- **Metal Pitch Shrinking**  
  - Lower metal pitch for tighter routing
- **Power Rail Optimization**  
  - Shift to **buried power rails (BPR)** for better utilization
- **Fin Depopulation**
  - Choose 2-fin or mixed-fin devices where possible

---

## Typical Library Variants

| Library Type | Target | Fin Count | Use Case |
|-------------|--------|-----------|---------|
| **HP (High Performance)** | Speed | 3–4 fins | CPU cores, high-speed logic |
| **HD (High Density)** | Area | 2 fins | Cache, memory periphery |
| **ULP (Ultra Low Power)** | Leakage | 2 fins, lower Vt | Always-on domains |

---

# 1.5 - Parasitic Resistance in Advanced CMOS Nodes

This repository documents **parasitic resistance**, its sources, impact on circuit performance, and methods for reduction.  
As technology nodes scale to **7nm, 5nm, and beyond**, parasitic resistance has become a major limiter of transistor and interconnect performance.

---

## What is Parasitic Resistance?

**Parasitic resistance** refers to unwanted series resistance present in a transistor or interconnect path.  
It does not contribute to useful functionality but degrades **drive current (Idsat)**, **speed**, and **power efficiency**.

---

## Sources of Parasitic Resistance

Parasitic resistance can be broken down into:

### 1. Device-Level Resistance
- **R<sub>S/D</sub>** – Source/Drain resistance
- **R<sub>C</sub>** – Contact resistance between metal and semiconductor
- **R<sub>ch,ext</sub>** – Extension region resistance (between contact and channel)
- **R<sub>spreading</sub>** – Resistance due to current crowding near the contact

### 2. Interconnect-Level Resistance
- **R<sub>line</sub>** – Resistance of metal lines (increases with shrinking dimensions)
- **Barrier/Liner contribution** – Higher share in narrow wires → higher effective resistivity
- **Via resistance** – Contribution from vertical interconnects between layers

---

## Impact on Performance

- ⬇ **Drive Current (I<sub>ON</sub>)** – Higher R lowers transistor performance  
- ⬇ **Switching Speed** – Increases delay (RC time constant)  
- ⬆ **Dynamic Power** – More voltage headroom required to maintain performance  
- ⬆ **IR Drop in Power Grid** – Reduces available supply voltage at cell level  

---

## Mitigation Techniques

### At Device Level
- **Silicidation Optimization** – Lower contact resistivity (NiSi, CoSi₂, Ru-based contacts)
- **Raised Source/Drain (RSD)** – Larger cross-sectional area → lower R
- **Epitaxial Engineering** – Stress engineering to improve mobility and reduce Rs
- **Advanced Contacts** – Semi-metallic or 2D contact materials to reduce Rc

### At Interconnect Level
- **Alternative Metals** – Ruthenium (Ru), Cobalt (Co), Mo-based materials
- **Barrier-Less or Thin Barrier Integration** – Reduce resistive liner fraction
- **Air-Gaps & Low-k Dielectrics** – Reduce parasitic capacitance and RC delay
- **Backside Power Delivery** – Dedicated low-resistance power routing

# 1.6 - Device Scaling Using Layered Materials

This repository explores **device scaling using layered (2D) materials** — such as MoS₂, WS₂, WSe₂, and graphene — as a path to extend Moore’s Law beyond the limits of traditional silicon FinFETs.

---

## Introduction

As silicon approaches its scaling limits at <5nm technology nodes, **layered materials** have emerged as a promising solution due to their:

- **Atomically thin channels** – excellent electrostatic control  
- **High carrier mobility** – faster switching and lower power  
- **Scalability** – ideal for Gate-All-Around (GAA) FET architectures  
- **Compatibility** – potential for heterogeneous integration with silicon CMOS  

---

## Why Layered Materials?

| Challenge in Si Scaling        | How 2D Materials Help |
|--------------------------------|----------------------|
| Short-channel effects (SCEs)   | Atomically thin body improves gate control |
| Variability due to doping      | 2D channels can be electrostatically doped |
| High contact resistance (Rc)   | Edge contacts and metal work-function engineering reduce Rc |
| Power dissipation              | Lower V<sub>DD</sub> operation possible |

---

## Device Architectures

Layered materials enable novel transistor designs:

- **2D FETs (MOSFET-like)** – Channel made of MoS₂, WSe₂, etc.  
- **GAAFET with 2D channel** – Gate-all-around for ultimate electrostatics  
- **2D TFETs** – Tunnel FETs using heterostructures for sub-60 mV/dec operation  
- **2D/3D Heterointegration** – Monolithic stacking with silicon for hybrid chips  

---

## Fabrication Challenges

- **Large-Area Growth** – Uniform wafer-scale CVD growth of 2D materials  
- **Contact Resistance** – Achieving low-resistance ohmic contacts  
- **Variability & Defects** – Controlling grain boundaries, vacancies  
- **Integration with BEOL** – Thermal budget compatibility with CMOS processes  

---

## Research Directions

- **Material Synthesis** – High-quality monolayer and few-layer growth  
- **Contact Engineering** – 1D edge contacts, phase-engineered contacts  
- **Dielectric Interface** – High-k gate stacks with minimal traps  
- **Strain Engineering** – Mobility enhancement via strain tuning  
- **Monolithic 3D Integration** – Stacking 2D devices for ultra-high density  

---

## Electrical Properties Investigated
The key electrical characteristics analyzed in this project include:

- **Carrier Mobility (µ):** Measures how quickly electrons or holes move through the material.
- **Threshold Voltage (Vth):** Voltage at which the device switches from off to on.
- **On/Off Current Ratio (Ion/Ioff):** Ratio of current in the on-state to the off-state; crucial for digital switches.
- **Subthreshold Swing (SS):** Indicates how effectively the device turns off; lower values are better.
- **Contact Resistance (Rc):** Resistance at the interface between metal contacts and layered materials.
- **Capacitance (C):** Gate capacitance influencing switching speed and power.
- **Parasitic Effects:** Includes series resistance, leakage currents, and capacitance contributions.

# 1.7 - 3D Structures in Device Scaling Using Layered Materials

## Overview
This repository explores **3D device structures** using layered materials for next-generation electronics. 3D structures improve **device density, performance, and scaling potential**, overcoming limitations of traditional planar devices.

## 3D Structures Investigated
The following 3D architectures are considered:

1. **FinFET (Fin Field-Effect Transistor)**  
   - 3D fin-like channel structure for better electrostatic control.  
   - Reduces short-channel effects.  
   - Materials: MoS₂, graphene.

2. **Gate-All-Around (GAA) FET**  
   - Channel completely surrounded by gate.  
   - Excellent subthreshold swing and leakage control.

3. **Vertical FET (VFET)**  
   - Vertical current flow for high-density integration.  
   - Minimizes footprint while maximizing current drive.

4. **Nanowire FET**  
   - Cylindrical 1D channels for uniform electrostatics.  
   - Can be stacked in 3D arrays.

5. **Stacked 2D Material Heterostructure**  
   - Multiple 2D layers stacked vertically (e.g., MoS₂/h-BN/Graphene).  
   - Enables vertical transport and tunneling devices.

6. **3D NAND Flash Structures**  
   - Vertical memory cells using layered materials.  
   - High storage density with scalable architecture.

7. **Vertical Tunnel FET (TFET)**  
   - Exploits band-to-band tunneling in vertical orientation.  
   - Ultra-low power consumption potential.

## Electrical Properties
Key parameters analyzed for these 3D structures:

| Structure | Carrier Mobility (cm²/V·s) | Ion/Ioff | Vth (V) | Subthreshold Swing (mV/dec) | Contact Resistance (Ω·µm) |
|-----------|---------------------------|----------|---------|----------------------------|---------------------------|
| FinFET    | 200                       | 1e6      | 0.3     | 65                         | 100                       |
| GAA FET   | 180                       | 1e7      | 0.25    | 60                         | 90                        |
| VFET      | 150                       | 1e5      | 0.35    | 70                         | 120                       |
| Nanowire  | 250                       | 1e6      | 0.3     | 55                         | 80                        |
| Stacked 2D| 300                       | 1e7      | 0.2     | 50                         | 70                        |
| 3D NAND   | 100                       | 1e4      | 0.4     | 80                         | 150                       |
| Vertical TFET| 220                    | 1e6      | 0.15    | 40                         | 60                        |

---

# Transistor-Level Monolithic 3D Integration Using Layered Materials

## Overview
This repository explores **monolithic 3D (M3D) integration** at the **transistor level** using layered materials such as MoS₂, graphene, and h-BN.  
M3D allows **stacking multiple transistor layers** vertically on a single chip, improving **device density, performance, and energy efficiency** without relying on traditional interconnect scaling.

## Key Concepts
- **Monolithic 3D Integration:** Vertical stacking of active transistor layers with dense inter-layer connections.  
- **Layered Materials:** 2D materials with high carrier mobility, tunable bandgap, and atomically thin channels.  
- **Benefits:**  
  - Reduced footprint and interconnect delay  
  - Higher transistor density  
  - Enhanced performance-per-watt  
  - Better scaling potential compared to 2D planar designs  

## Device Structures
The following transistor-level 3D architectures are considered:

1. **Stacked FinFETs (3D FinFETs)**  
   - Multiple FinFET layers stacked vertically.  
   - Shared substrate reduces interconnect length.  

2. **Gate-All-Around (GAA) M3D FETs**  
   - Vertically stacked nanowire channels completely surrounded by gates.  
   - Improved electrostatic control.

3. **Vertical Tunnel FETs (v-TFETs)**  
   - Exploits band-to-band tunneling across vertically aligned layers.  
   - Ultra-low-power switching.

4. **Heterostructure 3D FETs**  
   - Stacked layers of different 2D materials (e.g., MoS₂ on h-BN on Graphene) for optimized transport and performance.

## Electrical Properties
| Structure | Mobility (cm²/V·s) | Ion/Ioff | Threshold Voltage (V) | Subthreshold Swing (mV/dec) | Contact Resistance (Ω·µm) |
|-----------|-------------------|----------|----------------------|----------------------------|---------------------------|
| 3D FinFET | 220               | 1e6      | 0.3                  | 65                         | 100                       |
| GAA M3D FET | 200             | 1e7      | 0.25                 | 60                         | 90                        |
| Vertical TFET | 250            | 1e6      | 0.15                 | 40                         | 70                       |
| Heterostructure 3D FET | 300   | 1e7      | 0.2                  | 50                         | 60                        |

---

# Area Savings in Device Scaling Using Layered Materials

## Overview
This repository explores **area savings** achieved by **device scaling and 3D integration** using layered materials (e.g., MoS₂, graphene, h-BN).  
Area savings are critical in modern electronics to increase **device density, reduce interconnect length, and improve performance-per-watt**.

## Key Concepts
- **Device Scaling:** Reducing transistor dimensions while maintaining performance.  
- **3D Integration:** Stacking multiple device layers vertically to save chip area.  
- **Layered Materials:** Atomically thin materials allow high-density vertical integration.  
- **Benefits:**  
  - Higher transistor density per unit area  
  - Reduced interconnect overhead  
  - Improved energy efficiency  
  - Enabling of multi-functional circuits in compact footprint  

## Area Savings Analysis
| Device Architecture       | Planar Area (µm²) | 3D Stacked Area (µm²) | % Area Reduction |
|---------------------------|-----------------|----------------------|----------------|
| FinFET                    | 0.25            | 0.10                 | 60%            |
| Gate-All-Around (GAA) FET | 0.30           | 0.12                 | 60%            |
| Vertical TFET (v-TFET)    | 0.20            | 0.08                 | 60%            |
| Heterostructure 3D FET    | 0.35            | 0.14                 | 60%            |
| Monolithic 3D Stacked Devices | 0.50        | 0.18                 | 64%            |

**Notes:**  
- Vertical stacking reduces footprint significantly while maintaining or improving device performance.  
- Layered materials allow ultra-thin channels, enabling tight packing without short-channel degradation.  

---

# Monolithic 3D Circuits Using Layered Materials

## Overview
This repository explores **monolithic 3D (M3D) circuits** using layered materials like **MoS₂, graphene, and h-BN**.  
Monolithic 3D circuits stack **active transistor layers vertically**, enabling:

- Higher **device density**  
- Reduced **interconnect length and delay**  
- Improved **energy efficiency**  
- Enhanced **scalability** for next-generation electronics  

## Key Concepts
- **Monolithic 3D Integration:** Vertical stacking of multiple transistor layers on a single substrate.  
- **Layered Materials:** Atomically thin materials provide high mobility and low short-channel effects.  
- **Advantages:**  
  - Compact footprint with dense circuit layouts  
  - Reduced parasitic capacitance  
  - Improved performance-per-watt  
  - Compatibility with heterogeneous devices  

## Circuit Architectures
1. **Stacked FinFET Circuits**  
   - Vertically stacked FinFETs for dense digital logic.  

2. **Gate-All-Around (GAA) 3D Circuits**  
   - Vertical nanowire channels fully surrounded by gate for high performance.  

3. **Vertical Tunnel FET (v-TFET) Circuits**  
   - Exploit band-to-band tunneling for ultra-low-power logic.  

4. **Heterostructure 3D Circuits**  
   - Vertically stacked different 2D materials to optimize performance and functionality.  

## Electrical & Performance Benefits
| Circuit Type         | Density (Transistors/mm²) | Ion/Ioff | Subthreshold Swing (mV/dec) | Power Savings (%) |
|---------------------|--------------------------|----------|----------------------------|-----------------|
| Stacked FinFET      | 1.2M                     | 1e6      | 65                         | 30              |
| GAA 3D Circuits     | 1.5M                     | 1e7      | 60                         | 35              |
| Vertical TFET       | 1.0M                     | 1e6      | 40                         | 50              |
| Heterostructure 3D  | 1.6M                     | 1e7      | 50                         | 40              |

**Highlights:**  
- Monolithic 3D circuits reduce chip area by stacking transistors vertically.  
- Power efficiency improves due to shorter interconnects and optimized device design.  
- Layered materials enhance mobility and device switching performance.

  ---

  ## Overview
This repository focuses on **interconnect design and optimization** in **monolithic 3D (M3D) circuits** built with **layered materials** (MoS₂, graphene, h-BN).  
Interconnects play a critical role in **performance, power, and reliability** of densely stacked 3D circuits.

## Key Concepts
- **Interconnects in M3D Circuits:** Electrical connections linking vertically stacked transistors and layers.  
- **Challenges:**  
  - Increased resistance and capacitance due to vertical stacking  
  - Signal delay and cross-talk  
  - Thermal management in multi-layer structures  
- **Solutions:**  
  - Use of low-resistivity metals (Cu, Au) or graphene-based interconnects  
  - Optimized via density and placement  
  - Layered dielectrics (e.g., h-BN) to reduce parasitic capacitance  

## Interconnect Types
1. **Vertical Vias (Through-Layer Connections)**  
   - Connect transistors across stacked layers.  
   - Minimized via size improves area efficiency.  

2. **Horizontal Interconnects**  
   - Connect transistors within the same layer.  
   - Optimized routing reduces RC delay.  

3. **Hybrid Interconnects**  
   - Combination of metal and graphene for high performance and low resistance.  

## Electrical Properties & Performance
| Interconnect Type | Resistance (Ω/µm) | Capacitance (fF/µm) | Delay (ps) | Reliability Notes |
|-----------------|------------------|-------------------|------------|----------------|
| Cu Vias         | 0.1              | 0.05              | 5          | Sensitive to electromigration |
| Graphene Vias   | 0.05             | 0.03              | 3          | High thermal conductivity |
| Horizontal Metal | 0.2             | 0.06              | 6          | Standard metal lines |
| Hybrid (Metal+Graphene) | 0.08     | 0.04              | 4          | Optimized for low RC delay |

---
# Extending Copper Interconnects in Monolithic 3D Circuits

## Overview
This repository explores strategies for **extending and optimizing copper (Cu) interconnects** in **monolithic 3D (M3D) circuits** using layered materials (MoS₂, graphene, h-BN).  
Copper remains a standard choice for interconnects due to its **low resistivity and high conductivity**, but scaling 3D circuits requires careful design to minimize **RC delay, electromigration, and reliability issues**.

## Challenges with Copper Interconnects
- **Resistance increase** in long or narrow interconnects  
- **Capacitive coupling** between dense metal lines  
- **Electromigration** under high current density  
- **Thermal issues** in stacked layers  
- **Integration with layered materials** and ultra-thin transistors  

## Strategies for Extending Copper Interconnects
1. **Optimized Geometry**  
   - Wider or thicker Cu lines reduce resistance.  
   - Aspect ratio tuning for vias to minimize RC delay.

2. **Hybrid Interconnects**  
   - Combine Cu with graphene or other 2D materials for reduced resistance and improved thermal conductivity.  

3. **Low-k Dielectrics**  
   - Reduce capacitance between interconnects using materials like SiCOH or h-BN.  

4. **Electromigration Mitigation**  
   - Grain engineering and barrier layers to improve Cu reliability.  
   - Current density limits enforced in design rules.  

5. **Multi-Level 3D Routing**  
   - Use vertical stacking with multiple Cu layers and vias for dense circuits while maintaining performance.  

## Electrical Properties & Performance
| Interconnect Type       | Resistance (Ω/µm) | Capacitance (fF/µm) | Delay (ps) | Reliability Notes                  |
|------------------------|------------------|-------------------|------------|----------------------------------|
| Standard Cu Line        | 0.12             | 0.06              | 6          | Susceptible to electromigration  |
| Thick Cu Line           | 0.08             | 0.06              | 4          | Improved current handling        |
| Cu + Graphene Hybrid    | 0.05             | 0.04              | 3          | High thermal conductivity        |
| Cu via with Barrier     | 0.10             | 0.05              | 5          | Mitigates electromigration       |

---

# Non-Cu Metals in Monolithic 3D Circuits

## Overview
This repository explores the use of **non-copper (non-Cu) metals** for interconnects in **monolithic 3D (M3D) circuits** using layered materials (MoS₂, graphene, h-BN).  
While copper is standard, **alternative metals** like **Aluminum (Al), Tungsten (W), Cobalt (Co), and Molybdenum (Mo)** offer benefits in **reliability, high-temperature operation, and reduced electromigration**, especially for vertical 3D integration.

## Challenges with Copper
- Electromigration at high current densities  
- Limited thermal stability in 3D stacks  
- Compatibility issues with certain layered dielectrics  

## Advantages of Non-Cu Metals
| Metal | Resistivity (µΩ·cm) | Melting Point (°C) | Key Benefits | Applications in 3D ICs |
|-------|--------------------|------------------|-------------|------------------------|
| Aluminum (Al) | 2.82 | 660 | Low cost, easy deposition | Horizontal interconnects, vias |
| Tungsten (W) | 5.60 | 3422 | High melting point, low diffusion | Vertical vias, thermal robust layers |
| Cobalt (Co) | 6.24 | 1495 | Good electromigration resistance | High current density vias |
| Molybdenum (Mo) | 5.34 | 2623 | Stable at high temperature | Barrier layers, hybrid interconnects |
| Nickel (Ni) | 6.84 | 1455 | Corrosion-resistant, good adhesion | Thin interconnects, metallization layers |

## Integration Strategies
1. **Vertical Vias with W or Co**  
   - Ensures reliability under high current density and thermal stress.  

2. **Hybrid Interconnects**  
   - Combine Cu with non-Cu metals for optimized RC and reliability.  

3. **Barrier Layers**  
   - Use Mo or W as diffusion barriers between interconnects and layered dielectrics.  

4. **High-Temperature Operation**  
   - Non-Cu metals maintain integrity in stacked 3D ICs where thermal budgets are constrained.  

---

# Backside Power Delivery Network (BS-PDN) in Monolithic 3D Circuits

## Overview
This repository focuses on **Backside Power Delivery Networks (BS-PDNs)** for **monolithic 3D (M3D) circuits** using layered materials like MoS₂, graphene, and h-BN.  
BS-PDN provides **efficient power distribution** from the back side of the wafer, enabling:

- Reduced voltage drop (IR drop)  
- Improved current density handling  
- Lower noise and better signal integrity  
- Compact integration in 3D stacked circuits  

## Key Concepts
- **Backside Power Delivery Network (BS-PDN):** Power routing infrastructure placed on the wafer's back side.  
- **Benefits in 3D ICs:**  
  - Eliminates congestion in front-side routing  
  - Reduces thermal hotspots  
  - Enables denser transistor stacking without compromising power integrity  

## BS-PDN Components
1. **Vertical Vias / Through-Layer Vias (TLVs)**  
   - Connect back-side PDN to front-side transistors.  
   - Critical for low-resistance current delivery.

2. **Power Rails**  
   - Horizontal metal layers on the back side for VDD/VSS distribution.  
   - Can use Cu, W, or hybrid interconnects.

3. **Decoupling Capacitors**  
   - Minimize voltage fluctuations and stabilize power supply.

4. **Layered Dielectrics**  
   - h-BN or low-k dielectrics reduce parasitic capacitance and cross-talk.  

## Electrical Properties & Performance
| Parameter                  | Typical Value | Notes |
|----------------------------|---------------|-------|
| IR Drop                     | <50 mV        | Across stacked transistors |
| Via Resistance              | 0.05–0.1 Ω/µm | TLVs connecting BS-PDN to active layers |
| Current Density             | 10–20 MA/cm²  | Depending on Cu or W vias |
| Power Supply Noise Reduction| 30–50%       | With decoupling capacitors and optimized layout |
