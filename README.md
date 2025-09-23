# FinFETs_7nm_VSD
# 🔬 FinFET Circuit Design and Characterization  
### Device Models to 7nm Circuits (ASAP7)

This repository documents a **10-day intensive workshop** on **FinFET design and characterization** using **ASAP7 (7 nm PDK)** with **Xschem** and **Ngspice**.  
It includes **device modeling, inverter design, VTC extraction, noise margins, bandgap reference design, and PVT characterization** workflows.  

---

## 📅 Workshop Duration
**10 Days** – Hands-on, project-based training.  

---

## 📘 Learning Outcomes
By the end of this workshop, you will be able to:  
- Characterize **NFET/PFET** devices (Id–Vd, gm, ro).  
- Design and size a **7nm CMOS Inverter**.  
- Extract **VTC curves** and compute **noise margins**.  
- Automate simulations using **.measure scripts**.  
- Simulate a **Self-Cascode MOS Bandgap Reference**:
  - Generate **Vref**  
  - Analyze **line/load regulation**  
  - Evaluate **temperature drift**  
- Perform **PVT sweeps** for deterministic benchmarking.  
- Generate **publication-ready plots**.  

---

## 🛠️ Tools & Dependencies
- [Xschem](https://xschem.sourceforge.io/stefan/index.html) – Schematic capture  
- [Ngspice](http://ngspice.sourceforge.net/) – Circuit simulation  
- [ASAP7 PDK](https://github.com/The-OpenROAD-Project/asap7) – 7 nm device models  
- Python (for plotting & automation)  

Install Ngspice:  
```bash
sudo apt-get install ngspice
