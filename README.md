## FinFET Circuit Design and Characterization
This GitHub repository documents the 10-day workshop on FinFET Circuit Design and Characterization using ASAP7 PDK offered by VSD Corp. Pvt. Ltd. attended from 10 Sep - 19 Sept, 2025.

## Table of Contents

| Module | Topics Covered |
|--------|----------------|
| 1. Scaling Beyond CMOS  | - Introduction to FinFets <br> - Device Scaling Using Layered Materials <br> - FEOL Innovations <br> - 3D Structures |
| 2. 7nm FinFET  | - 7nm FinFet Nmos <br> - Performance Analysis <br> -  7nm Inverter Characterization |
| 3. BGR Circuit  | - Bandagap Reference Circuit <br> - BGRef Characterization |


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

  Unit Scale (to Compute)
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
- Uniform atomic scale thickness (thickness scaling limit (~0.65nm MoS₂ monolayer) 
- Effective mass m* higher (~0.55 mo for MoS₂ compared to ~0.22 mo for silicon)  
- Bandgap (eg MoS₂ monolayer ~1.85ev, MoS₂ bilayer ~1.5ev)

<img width="1259" height="666" alt="Screenshot 2025-09-16 012833" src="https://github.com/user-attachments/assets/14bcb6e3-9738-4223-9732-e5076d6e4b57" />

---

Transistor Scaling to sub-5nm Gate Lengths

Transistor scaling for higher packing density, better performance, lower cost.

Challenges for scaling

- Direct source-to-drain tunneling leakage, need high effective mass (m*).
- Surface roughness and thickness variations, uniform atomically thin materials.
- CD high relative to Cox, need low-in plane dielectric constant (ε) and new channel material.
  
---

Direct Source-to_Drain Tunneling

- Up to 100x reduction in direct source to drain tunneling leakage due to higher m*, Larger Eg and lower ε of MoS₂ relative to silicon.
- Large energy savings in electronics.
 
<img width="2358" height="985" alt="Screenshot 2025-09-16 013236" src="https://github.com/user-attachments/assets/35891953-0ea0-4f38-b35f-39cf682bf439" />

---

 MoS₂ Transistor with 1nm Gate Length

-  1nm single walled carbon nanotube gate with MoS₂ channel.
-  Shortest gate length transistor demonstarted.
-  MoS₂ extensions inverted using gloabl si back gate and CNT gate depletes a small region of MoS₂ above it.
-  Large energy savings in electronics.
    
---

## 1.8 3D-Structures

Body-Bias Effect - very challenging to form single-crystalline semiconductor of non-planar surface using conventional semiconductors.

<img width="560" height="566" alt="Screenshot 2025-09-16 020551" src="https://github.com/user-attachments/assets/9052a14f-9da2-48c5-940d-191fdec85210" />

---

Electrical Characteristics

- Short-channel MoS₂ FET Lg=50nm
- Excellent short-channel performance
- Enhanced back-bais effect

<img width="1626" height="1067" alt="Screenshot 2025-09-16 020938" src="https://github.com/user-attachments/assets/1fbd88b6-9ff2-43d9-ad37-ddf9966bcfb0" />

---

Transistor-Level Monolithic 3D

<img width="1707" height="1026" alt="Screenshot 2025-09-16 021006" src="https://github.com/user-attachments/assets/d30324b8-88d3-4439-9a62-ca84e8eeb5ed" />

---

Area Savings

<img width="1122" height="481" alt="Screenshot 2025-09-16 021125" src="https://github.com/user-attachments/assets/0527d7c0-803a-4975-9e71-f2192160a3e9" />

---

Monolithic 3D Circuits

<img width="1260" height="1000" alt="Screenshot 2025-09-16 021143" src="https://github.com/user-attachments/assets/db289a24-80ce-4739-a057-0499543bccf4" />

---

Interconnects

<img width="2572" height="1311" alt="Screenshot 2025-09-16 021844" src="https://github.com/user-attachments/assets/4f215f59-6dc4-414d-9dc4-d0068e64212d" />

---

Extending Copper Interconnects

<img width="2457" height="1361" alt="Screenshot 2025-09-16 021912" src="https://github.com/user-attachments/assets/e64093ef-69ac-4301-96e6-2c5649576ea5" />

---

Non Cu-Metals
- Some potential candidates :- Rh, Ir, Mo, Ni, Co and Ru
- λ×P₀ is an indicator for size-effect / electron scattering at small interconnect dimensions.
- Higher melting temperature / cohesive energy for EM elimination.
- Required linear thickness will impact conductor volume and line R at small dimensions.
- New post Cu-candidates must be barrier-less. (with sub-nm adhesion / seed layer)

<img width="974" height="914" alt="Screenshot 2025-09-16 021936" src="https://github.com/user-attachments/assets/cd966860-1623-4bd3-ac25-57cc6a27a10b" />

---

Back-side Power Delivery Network (Bs-PDN)

<img width="3220" height="1536" alt="Screenshot 2025-09-16 021956" src="https://github.com/user-attachments/assets/0f7dc32e-e089-4bfb-823e-c45c02eb76ba" />

---

## 2.1 7nm FinFET Nmos Performance Analysis

<details> <summary> <b>SPICE Deck:</b> nfet_char.spice </summary>

```
** sch_path: /home/vsduser/Desktop/nfetchar.sch
**.subckt nfetchar
Xnfet1 nfet_out nfet_in GND GND asap_7nm_nfet l=7e-009 nfin=14
R1 vdd nfet_out 1k m=1
V1 nfet_in GND 3
V2 VDD GND 3
**** begin user architecture code

 .dc v1 0 0.7 1m v2 0 0.7 0.2
.control
run
set xbrushwidth=3
let vd = vdd - nfet_out
let id  = vd/1000
plot id
.endc

**** end user architecture code
**.ends
.GLOBAL GND
.GLOBAL VDD
.GLOBAL nfet_in
**** begin user architecture code

.subckt asap_7nm_nfet S G D B l=7e-009 nfin=14
	nnmos_finfet S G D B BSIMCMG_osdi_N l=7e-009 nfin=14
.ends asap_7nm_nfet

.model BSIMCMG_osdi_N BSIMCMG_va (
+ TYPE = 1
************************************************************
*                         general                          *
************************************************************
+version = 107             bulkmod = 1               igcmod  = 1               igbmod  = 0
+gidlmod = 1               iimod   = 0               geomod  = 1               rdsmod  = 0
+rgatemod= 0               rgeomod = 0               shmod   = 0               nqsmod  = 0
+coremod = 0               cgeomod = 0               capmod  = 0               tnom    = 25
+eot     = 1e-009          eotbox  = 1.4e-007        eotacc  = 1e-010          tfin    = 6.5e-009
+toxp    = 2.1e-009        nbody   = 1e+022          phig    = 4.2466          epsrox  = 3.9
+epsrsub = 11.9            easub   = 4.05            ni0sub  = 1.1e+016        bg0sub  = 1.17
+nc0sub  = 2.86e+025       nsd     = 2e+026          ngate   = 0               nseg    = 5
+l       = 2.1e-008        xl      = 1e-009          lint    = -2e-009         dlc     = 0
+dlbin   = 0               hfin    = 3.2e-008        deltaw  = 0               deltawcv= 0
+sdterm  = 0               epsrsp  = 3.9             nfin    = 1
+toxg    = 1.80e-009
************************************************************
*                            dc                            *
************************************************************
+cit     = 0               cdsc    = 0.01            cdscd   = 0.01            dvt0    = 0.05
+dvt1    = 0.47            phin    = 0.05            eta0    = 0.07            dsub    = 0.35
+k1rsce  = 0               lpe0    = 0               dvtshift= 0               qmfactor= 2.5
+etaqm   = 0.54            qm0     = 0.001           pqm     = 0.66            u0      = 0.0303
+etamob  = 2               up      = 0               ua      = 0.55            eu      = 1.2
+ud      = 0               ucs     = 1               rdswmin = 0               rdsw    = 200
+wr      = 1               rswmin  = 0               rdwmin  = 0               rshs    = 0
+rshd    = 0               vsat    = 70000           deltavsat= 0.2             ksativ  = 2
+mexp    = 4               ptwg    = 30              pclm    = 0.05            pclmg   = 0
+pdibl1  = 0               pdibl2  = 0.002           drout   = 1               pvag    = 0
+fpitch  = 2.7e-008        rth0    = 0.225           cth0    = 1.243e-006      wth0    = 2.6e-007
+lcdscd  = 5e-005          lcdscdr = 5e-005          lrdsw   = 0.2             lvsat   = 0
************************************************************
*                         leakage                          *
************************************************************
+aigc    = 0.014           bigc    = 0.005           cigc    = 0.25            dlcigs  = 1e-009
+dlcigd  = 1e-009          aigs    = 0.0115          aigd    = 0.0115          bigs    = 0.00332
+bigd    = 0.00332         cigs    = 0.35            cigd    = 0.35            poxedge = 1.1
+agidl   = 1e-012          agisl   = 1e-012          bgidl   = 10000000        bgisl   = 10000000
+egidl   = 0.35            egisl   = 0.35
************************************************************
*                            rf                            *
************************************************************
************************************************************
*                         junction                         *
************************************************************
************************************************************
*                       capacitance                        *
************************************************************
+cfs     = 0               cfd     = 0               cgso    = 1.6e-010        cgdo    = 1.6e-010
+cgsl    = 0               cgdl    = 0               ckappas = 0.6             ckappad = 0.6
+cgbo    = 0               cgbl    = 0
************************************************************
*                       temperature                        *
************************************************************
+tbgasub = 0.000473        tbgbsub = 636             kt1     = 0               kt1l    = 0
+ute     = -0.7            utl     = 0               ua1     = 0.001032        ud1     = 0
+ucste   = -0.004775       at      = 0.001           ptwgt   = 0.004           tmexp   = 0
+prt     = 0               tgidl   = -0.007          igt     = 2.5
************************************************************
*                          noise                           *
************************************************************
**)
.control
pre_osdi /home/vsduser/Downloads/bsimcmg.osdi
.endc


**** end user architecture code
.end 
```
</details>

Schematic of nfet in Xschem

![WhatsApp Image 2025-09-24 at 11 55 30 PM (1)](https://github.com/user-attachments/assets/c8846bb8-7255-4e70-95a1-8e0a1edac317)


<details> <summary> <b>SPICE Deck:</b> nfet_char2.spice </summary>

```
** sch_path: /home/vsduser/Desktop/asap_7nm_Xschem/inverter_7nmfinfet.sch
**.subckt inverter_7nmfinfet
Xnfet1 nfet_out nfet_in GND GND asap_7nm_nfet l=7e-009 nfin=14
Xpfet1 nfet_out nfet_in vdd vdd asap_7nm_pfet l=7e-009 nfin=14
V1 nfet_in GND pulse(0 0.7 20p 10p 10p 20p 500p 1)
V2 vdd GND 0.7
**** begin user architecture code


.tran 0.1p 100p
.control
    run
    set xbrushwidth=3
    plot nfet_out nfet_in
.endc


**** end user architecture code
**.ends
.GLOBAL GND
**** begin user architecture code

.subckt asap_7nm_pfet S G D B l=7e-009 nfin=14
	npmos_finfet S G D B BSIMCMG_osdi_P l=7e-009 nfin=14
.ends asap_7nm_pfet

.model BSIMCMG_osdi_P BSIMCMG_va (
+ TYPE = 0

************************************************************
*                         general                          *
************************************************************
+version = 107             bulkmod = 1               igcmod  = 1               igbmod  = 0
+gidlmod = 1               iimod   = 0               geomod  = 1               rdsmod  = 0
+rgatemod= 0               rgeomod = 0               shmod   = 0               nqsmod  = 0
+coremod = 0               cgeomod = 0               capmod  = 0               tnom    = 25
+eot     = 1e-009          eotbox  = 1.4e-007        eotacc  = 3e-010          tfin    = 6.5e-009
+toxp    = 2.1e-009        nbody   = 1e+022          phig    = 4.9278          epsrox  = 3.9
+epsrsub = 11.9            easub   = 4.05            ni0sub  = 1.1e+016        bg0sub  = 1.17
+nc0sub  = 2.86e+025       nsd     = 2e+026          ngate   = 0               nseg    = 5
+l       = 2.1e-008        xl      = 1e-009          lint    = -2.5e-009       dlc     = 0
+dlbin   = 0               hfin    = 3.2e-008        deltaw  = 0               deltawcv= 0
+sdterm  = 0               epsrsp  = 3.9             nfin    = 1
+toxg    = 1.8e-009
************************************************************
*                            dc                            *
************************************************************
+cit     = 0               cdsc    = 0.003469        cdscd   = 0.001486        dvt0    = 0.05
+dvt1    = 0.36            phin    = 0.05            eta0    = 0.094           dsub    = 0.24
+k1rsce  = 0               lpe0    = 0               dvtshift= 0               qmfactor= 0
+etaqm   = 0.54            qm0     = 2.183e-012      pqm     = 0.66            u0      = 0.0237
+etamob  = 4               up      = 0               ua      = 1.133           eu      = 0.05
+ud      = 0.0105          ucs     = 0.2672          rdswmin = 0               rdsw    = 200
+wr      = 1               rswmin  = 0               rdwmin  = 0               rshs    = 0
+rshd    = 0               vsat    = 60000           deltavsat= 0.17            ksativ  = 1.592
+mexp    = 2.491           ptwg    = 25              pclm    = 0.01            pclmg   = 1
+pdibl1  = 800             pdibl2  = 0.005704        drout   = 4.97            pvag    = 200
+fpitch  = 2.7e-008        rth0    = 0.15            cth0    = 1.243e-006      wth0    = 2.6e-007
+lcdscd  = 0               lcdscdr = 0               lrdsw   = 1.3             lvsat   = 1441
************************************************************
*                         leakage                          *
************************************************************
+aigc    = 0.007           bigc    = 0.0015          cigc    = 1               dlcigs  = 5e-009
+dlcigd  = 5e-009          aigs    = 0.006           aigd    = 0.006           bigs    = 0.001944
+bigd    = 0.001944        cigs    = 1               cigd    = 1               poxedge = 1.152
+agidl   = 2e-012          agisl   = 2e-012          bgidl   = 1.5e+008        bgisl   = 1.5e+008
+egidl   = 1.142           egisl   = 1.142
************************************************************
*                            rf                            *
************************************************************
************************************************************
*                         junction                         *
************************************************************
************************************************************
*                       capacitance                        *
************************************************************
+cfs     = 0               cfd     = 0               cgso    = 1.6e-010        cgdo    = 1.6e-010
+cgsl    = 0               cgdl    = 0               ckappas = 0.6             ckappad = 0.6
+cgbo    = 0               cgbl    = 0
************************************************************
*                       temperature                        *
************************************************************
+tbgasub = 0.000473        tbgbsub = 636             kt1     = 0               kt1l    = 0
+ute     = -1.2            utl     = 0               ua1     = 0.001032        ud1     = 0
+ucste   = -0.004775       at      = 0.001           ptwgt   = 0.004           tmexp   = 0
+prt     = 0               tgidl   = -0.007          igt     = 2.5
************************************************************
*                          noise                           *
************************************************************
**)
.control
pre_osdi /home/vsduser/Desktop/asap_7nm_Xschem/bsimcmg.osdi
.endc



.subckt asap_7nm_nfet S G D B l=7e-009 nfin=14
	nnmos_finfet S G D B BSIMCMG_osdi_N l=7e-009 nfin=14
.ends asap_7nm_nfet

.model BSIMCMG_osdi_N BSIMCMG_va (
+ TYPE = 1
************************************************************
*                         general                          *
************************************************************
+version = 107             bulkmod = 1               igcmod  = 1               igbmod  = 0
+gidlmod = 1               iimod   = 0               geomod  = 1               rdsmod  = 0
+rgatemod= 0               rgeomod = 0               shmod   = 0               nqsmod  = 0
+coremod = 0               cgeomod = 0               capmod  = 0               tnom    = 25
+eot     = 1e-009          eotbox  = 1.4e-007        eotacc  = 1e-010          tfin    = 6.5e-009
+toxp    = 2.1e-009        nbody   = 1e+022          phig    = 4.2466          epsrox  = 3.9
+epsrsub = 11.9            easub   = 4.05            ni0sub  = 1.1e+016        bg0sub  = 1.17
+nc0sub  = 2.86e+025       nsd     = 2e+026          ngate   = 0               nseg    = 5
+l       = 2.1e-008        xl      = 1e-009          lint    = -2e-009         dlc     = 0
+dlbin   = 0               hfin    = 3.2e-008        deltaw  = 0               deltawcv= 0
+sdterm  = 0               epsrsp  = 3.9             nfin    = 1
+toxg    = 1.80e-009
************************************************************
*                            dc                            *
************************************************************
+cit     = 0               cdsc    = 0.01            cdscd   = 0.01            dvt0    = 0.05
+dvt1    = 0.47            phin    = 0.05            eta0    = 0.07            dsub    = 0.35
+k1rsce  = 0               lpe0    = 0               dvtshift= 0               qmfactor= 2.5
+etaqm   = 0.54            qm0     = 0.001           pqm     = 0.66            u0      = 0.0303
+etamob  = 2               up      = 0               ua      = 0.55            eu      = 1.2
+ud      = 0               ucs     = 1               rdswmin = 0               rdsw    = 200
+wr      = 1               rswmin  = 0               rdwmin  = 0               rshs    = 0
+rshd    = 0               vsat    = 70000           deltavsat= 0.2             ksativ  = 2
+mexp    = 4               ptwg    = 30              pclm    = 0.05            pclmg   = 0
+pdibl1  = 0               pdibl2  = 0.002           drout   = 1               pvag    = 0
+fpitch  = 2.7e-008        rth0    = 0.225           cth0    = 1.243e-006      wth0    = 2.6e-007
+lcdscd  = 5e-005          lcdscdr = 5e-005          lrdsw   = 0.2             lvsat   = 0
************************************************************
*                         leakage                          *
************************************************************
+aigc    = 0.014           bigc    = 0.005           cigc    = 0.25            dlcigs  = 1e-009
+dlcigd  = 1e-009          aigs    = 0.0115          aigd    = 0.0115          bigs    = 0.00332
+bigd    = 0.00332         cigs    = 0.35            cigd    = 0.35            poxedge = 1.1
+agidl   = 1e-012          agisl   = 1e-012          bgidl   = 10000000        bgisl   = 10000000
+egidl   = 0.35            egisl   = 0.35
************************************************************
*                            rf                            *
************************************************************
************************************************************
*                         junction                         *
************************************************************
************************************************************
*                       capacitance                        *
************************************************************
+cfs     = 0               cfd     = 0               cgso    = 1.6e-010        cgdo    = 1.6e-010
+cgsl    = 0               cgdl    = 0               ckappas = 0.6             ckappad = 0.6
+cgbo    = 0               cgbl    = 0
************************************************************
*                       temperature                        *
************************************************************
+tbgasub = 0.000473        tbgbsub = 636             kt1     = 0               kt1l    = 0
+ute     = -0.7            utl     = 0               ua1     = 0.001032        ud1     = 0
+ucste   = -0.004775       at      = 0.001           ptwgt   = 0.004           tmexp   = 0
+prt     = 0               tgidl   = -0.007          igt     = 2.5
************************************************************
*                          noise                           *
************************************************************
**)
.control
pre_osdi /home/vsduser/Desktop/asap_7nm_Xschem/bsimcmg.osdi
.endc


**** end user architecture code
.end
```
</details>

```bash
plot Id
```

![WhatsApp Image 2025-09-24 at 10 59 19 PM (1)](https://github.com/user-attachments/assets/78ed4562-8a4d-4875-966b-74508342dcee)

```bash
plot id vs vd
```

![WhatsApp Image 2025-09-24 at 10 59 19 PM](https://github.com/user-attachments/assets/c4481690-c0e2-43e1-a197-9ecc2f50a774)

## 2.2 CMOS Inverter_vtc Characteristics

<details> <summary> <b>SPICE Deck:</b> inverter_vtc.spice </summary>

```

** sch_path: /home/vsduser/Desktop/asap_7nm_Xschem/inverter_vtcchar.sch
**.subckt inverter_vtcchar
Xnfet1 nfet_out nfet_in GND GND asap_7nm_nfet l=7e-009 nfin=14
Xpfet1 nfet_out nfet_in vdd vdd asap_7nm_pfet l=7e-009 nfin=14
V1 nfet_in GND pulse(0 0.7 20p 10p 10p 20p 500p 1)
V2 vdd GND 0.7
**** begin user architecture code


.dc v1 0 0.7 1m
.control
    run
    set xbrushwidth=3
    plot nfet_out nfet_in
    meas dc v_th when nfet_out=nfet_in
.endc


**** end user architecture code
**.ends
.GLOBAL GND
**** begin user architecture code

.subckt asap_7nm_pfet S G D B l=7e-009 nfin=14
	npmos_finfet S G D B BSIMCMG_osdi_P l=7e-009 nfin=14
.ends asap_7nm_pfet

.model BSIMCMG_osdi_P BSIMCMG_va (
+ TYPE = 0

************************************************************
*                         general                          *
************************************************************
+version = 107             bulkmod = 1               igcmod  = 1               igbmod  = 0
+gidlmod = 1               iimod   = 0               geomod  = 1               rdsmod  = 0
+rgatemod= 0               rgeomod = 0               shmod   = 0               nqsmod  = 0
+coremod = 0               cgeomod = 0               capmod  = 0               tnom    = 25
+eot     = 1e-009          eotbox  = 1.4e-007        eotacc  = 3e-010          tfin    = 6.5e-009
+toxp    = 2.1e-009        nbody   = 1e+022          phig    = 4.9278          epsrox  = 3.9
+epsrsub = 11.9            easub   = 4.05            ni0sub  = 1.1e+016        bg0sub  = 1.17
+nc0sub  = 2.86e+025       nsd     = 2e+026          ngate   = 0               nseg    = 5
+l       = 2.1e-008        xl      = 1e-009          lint    = -2.5e-009       dlc     = 0
+dlbin   = 0               hfin    = 3.2e-008        deltaw  = 0               deltawcv= 0
+sdterm  = 0               epsrsp  = 3.9             nfin    = 1
+toxg    = 1.8e-009
************************************************************
*                            dc                            *
************************************************************
+cit     = 0               cdsc    = 0.003469        cdscd   = 0.001486        dvt0    = 0.05
+dvt1    = 0.36            phin    = 0.05            eta0    = 0.094           dsub    = 0.24
+k1rsce  = 0               lpe0    = 0               dvtshift= 0               qmfactor= 0
+etaqm   = 0.54            qm0     = 2.183e-012      pqm     = 0.66            u0      = 0.0237
+etamob  = 4               up      = 0               ua      = 1.133           eu      = 0.05
+ud      = 0.0105          ucs     = 0.2672          rdswmin = 0               rdsw    = 200
+wr      = 1               rswmin  = 0               rdwmin  = 0               rshs    = 0
+rshd    = 0               vsat    = 60000           deltavsat= 0.17            ksativ  = 1.592
+mexp    = 2.491           ptwg    = 25              pclm    = 0.01            pclmg   = 1
+pdibl1  = 800             pdibl2  = 0.005704        drout   = 4.97            pvag    = 200
+fpitch  = 2.7e-008        rth0    = 0.15            cth0    = 1.243e-006      wth0    = 2.6e-007
+lcdscd  = 0               lcdscdr = 0               lrdsw   = 1.3             lvsat   = 1441
************************************************************
*                         leakage                          *
************************************************************
+aigc    = 0.007           bigc    = 0.0015          cigc    = 1               dlcigs  = 5e-009
+dlcigd  = 5e-009          aigs    = 0.006           aigd    = 0.006           bigs    = 0.001944
+bigd    = 0.001944        cigs    = 1               cigd    = 1               poxedge = 1.152
+agidl   = 2e-012          agisl   = 2e-012          bgidl   = 1.5e+008        bgisl   = 1.5e+008
+egidl   = 1.142           egisl   = 1.142
************************************************************
*                            rf                            *
************************************************************
************************************************************
*                         junction                         *
************************************************************
************************************************************
*                       capacitance                        *
************************************************************
+cfs     = 0               cfd     = 0               cgso    = 1.6e-010        cgdo    = 1.6e-010
+cgsl    = 0               cgdl    = 0               ckappas = 0.6             ckappad = 0.6
+cgbo    = 0               cgbl    = 0
************************************************************
*                       temperature                        *
************************************************************
+tbgasub = 0.000473        tbgbsub = 636             kt1     = 0               kt1l    = 0
+ute     = -1.2            utl     = 0               ua1     = 0.001032        ud1     = 0
+ucste   = -0.004775       at      = 0.001           ptwgt   = 0.004           tmexp   = 0
+prt     = 0               tgidl   = -0.007          igt     = 2.5
************************************************************
*                          noise                           *
************************************************************
**)
.control
pre_osdi /home/vsduser/Desktop/asap_7nm_Xschem/bsimcmg.osdi
.endc



.subckt asap_7nm_nfet S G D B l=7e-009 nfin=14
	nnmos_finfet S G D B BSIMCMG_osdi_N l=7e-009 nfin=14
.ends asap_7nm_nfet

.model BSIMCMG_osdi_N BSIMCMG_va (
+ TYPE = 1
************************************************************
*                         general                          *
************************************************************
+version = 107             bulkmod = 1               igcmod  = 1               igbmod  = 0
+gidlmod = 1               iimod   = 0               geomod  = 1               rdsmod  = 0
+rgatemod= 0               rgeomod = 0               shmod   = 0               nqsmod  = 0
+coremod = 0               cgeomod = 0               capmod  = 0               tnom    = 25
+eot     = 1e-009          eotbox  = 1.4e-007        eotacc  = 1e-010          tfin    = 6.5e-009
+toxp    = 2.1e-009        nbody   = 1e+022          phig    = 4.2466          epsrox  = 3.9
+epsrsub = 11.9            easub   = 4.05            ni0sub  = 1.1e+016        bg0sub  = 1.17
+nc0sub  = 2.86e+025       nsd     = 2e+026          ngate   = 0               nseg    = 5
+l       = 2.1e-008        xl      = 1e-009          lint    = -2e-009         dlc     = 0
+dlbin   = 0               hfin    = 3.2e-008        deltaw  = 0               deltawcv= 0
+sdterm  = 0               epsrsp  = 3.9             nfin    = 1
+toxg    = 1.80e-009
************************************************************
*                            dc                            *
************************************************************
+cit     = 0               cdsc    = 0.01            cdscd   = 0.01            dvt0    = 0.05
+dvt1    = 0.47            phin    = 0.05            eta0    = 0.07            dsub    = 0.35
+k1rsce  = 0               lpe0    = 0               dvtshift= 0               qmfactor= 2.5
+etaqm   = 0.54            qm0     = 0.001           pqm     = 0.66            u0      = 0.0303
+etamob  = 2               up      = 0               ua      = 0.55            eu      = 1.2
+ud      = 0               ucs     = 1               rdswmin = 0               rdsw    = 200
+wr      = 1               rswmin  = 0               rdwmin  = 0               rshs    = 0
+rshd    = 0               vsat    = 70000           deltavsat= 0.2             ksativ  = 2
+mexp    = 4               ptwg    = 30              pclm    = 0.05            pclmg   = 0
+pdibl1  = 0               pdibl2  = 0.002           drout   = 1               pvag    = 0
+fpitch  = 2.7e-008        rth0    = 0.225           cth0    = 1.243e-006      wth0    = 2.6e-007
+lcdscd  = 5e-005          lcdscdr = 5e-005          lrdsw   = 0.2             lvsat   = 0
************************************************************
*                         leakage                          *
************************************************************
+aigc    = 0.014           bigc    = 0.005           cigc    = 0.25            dlcigs  = 1e-009
+dlcigd  = 1e-009          aigs    = 0.0115          aigd    = 0.0115          bigs    = 0.00332
+bigd    = 0.00332         cigs    = 0.35            cigd    = 0.35            poxedge = 1.1
+agidl   = 1e-012          agisl   = 1e-012          bgidl   = 10000000        bgisl   = 10000000
+egidl   = 0.35            egisl   = 0.35
************************************************************
*                            rf                            *
************************************************************
************************************************************
*                         junction                         *
************************************************************
************************************************************
*                       capacitance                        *
************************************************************
+cfs     = 0               cfd     = 0               cgso    = 1.6e-010        cgdo    = 1.6e-010
+cgsl    = 0               cgdl    = 0               ckappas = 0.6             ckappad = 0.6
+cgbo    = 0               cgbl    = 0
************************************************************
*                       temperature                        *
************************************************************
+tbgasub = 0.000473        tbgbsub = 636             kt1     = 0               kt1l    = 0
+ute     = -0.7            utl     = 0               ua1     = 0.001032        ud1     = 0
+ucste   = -0.004775       at      = 0.001           ptwgt   = 0.004           tmexp   = 0
+prt     = 0               tgidl   = -0.007          igt     = 2.5
************************************************************
*                          noise                           *
************************************************************
**)
.control
pre_osdi /home/vsduser/Desktop/asap_7nm_Xschem/bsimcmg.osdi
.endc


**** end user architecture code
.end

```
</details>

Inverter schematic in Xschem

<img width="1666" height="1018" alt="Screenshot 2025-09-25 000132" src="https://github.com/user-attachments/assets/4ae4fb32-ab58-4fd6-bd18-10c0b795dffb" />

## 2.3 Inverter Performance 

---

- VTC Curve (Vout vs. Vin)

Spice command for calculating V_th 
```bash
dc v_th when nfet_out=nfet_in
```
![WhatsApp Image 2025-09-24 at 10 59 20 PM](https://github.com/user-attachments/assets/fff1fccb-4d37-4e42-b7f5-2d3e931fb4ae)

- Drain Current (Id)

Spice command for Id
```bash
let id=v2#branch
plot id
```

<img width="915" height="817" alt="Screenshot 2025-09-24 234445" src="https://github.com/user-attachments/assets/b17b02cb-141e-4a42-a0d2-b7990d432843" />

- Gain (Av)

Spice command for Av
```bash
let gain_Av = abs(deriv(Vout))
plot gain_Av
```

![WhatsApp Image 2025-09-24 at 11 32 44 PM](https://github.com/user-attachments/assets/4fad4698-90bb-4282-bccb-88626d712111)

- Transconductance (Gm)

Spice command for Gm
```bash
let gm = real(deriv(id, nfet_in))
meas dc gm_max MAX gm
plot gm
```

![WhatsApp Image 2025-09-24 at 11 32 44 PM (1)](https://github.com/user-attachments/assets/ee1e91b0-f3a9-4362-9d06-832aef4fc510)

- Output Resistance (Rout)

Spice command for Rout
```bash
let r_out= deriv(nfet_out,id)  
plot r_out
```

![WhatsApp Image 2025-09-24 at 10 59 21 PM (1)](https://github.com/user-attachments/assets/ae2d20f0-8b4d-42f8-bbee-31b0faa1d544)

- Transient Analysis

Spice command for Transient Analysis
```bash
.param VDD_V    = 0.7
.csparam VDD_V  = 'VDD_V'
.csparam VLOW   = '0.2 * VDD_V'
.csparam VHIGH  = '0.8 * VDD_V'
```

<img width="596" height="500" alt="Screenshot 2025-09-24 234316" src="https://github.com/user-attachments/assets/0af51b04-23cf-4388-873c-5f6e4f0a1212" />



Values for switching threshold , drain current , Power , tpd , Av and frequency derived from graphs



![WhatsApp Image 2025-09-24 at 10 59 24 PM](https://github.com/user-attachments/assets/4349dfa6-e493-447e-88c6-33964d300645)

## 2.4 7nm FinFET Inverter Characterization

Schematic of Inverter

![WhatsApp Image 2025-09-25 at 12 07 44 AM](https://github.com/user-attachments/assets/8efb3783-7a12-4792-a15a-f97e1dd70f57)

Characterization Table

| S.No. | Nfin_P | W/L (PMOS) | W/L (NMOS) | Vth (V)   | Id (A)        | P (W)          | tpd (ps) | Av      | f (Hz)           |
|-------|--------|------------|------------|-----------|---------------|----------------|----------|---------|------------------|
| 1     | 7      | 2          | 2          | 0.3447875 | 8.07135×10^-7 | 2.964602×10^-5 | 25.30216 | 6.428412 | 2.246325×10^10 |
| 2     | 7      | 1.43       | 2          | 0.3215502 | 8.06808×10^-7 | 2.494137×10^-5 | 25.07247 | 6.482698 | 2.259247×10^10 |
| 3     | 7      | 1.57       | 2.14       | 0.3233583 | 8.64469×10^-7 | 2.710435×10^-5 | 25.08771 | 6.474671 | 2.258481×10^10 |
| 4     | 7      | 1.71       | 2.29       | 0.324903  | 9.22128×10^-7 | 2.926088×10^-5 | 25.10123 | 6.469781 | 2.257800×10^10 |
| 5     | 7      | 1.86       | 2.86       | 0.3151001 | 1.15242×10^-6 | 3.382684×10^-5 | 25.02181 | 6.512160 | 2.261735×10^10 |
| 6     | 7      | 2.86       | 1.71       | 0.3646163 | 6.92006×10^-7 | 2.907917×10^-5 | 25.46383 | 6.446225 | 2.228250×10^10 |
| 7     | 7      | 2.14       | 1.71       | 0.3601895 | 6.91971×10^-7 | 2.823814×10^-5 | 25.42951 | 6.437911 | 2.232961×10^10 |
| 8     | 7      | 2          | 1.71       | 0.3554406 | 6.91931×10^-7 | 2.734615×10^-5 | 25.39228 | 6.431933 | 2.237567×10^10 |
| 9     | 7      | 1.86       | 1.71       | 0.3503247 | 6.91884×10^-7 | 2.641482×10^-5 | 25.35068 | 6.427584 | 2.242034×10^10 |
| 10    | 7      | 1.71       | 1.71       | 0.3447875 | 6.9183×10^-7  | 2.541088×10^-5 | 25.30216 | 6.428412 | 2.246325×10^10 |
| 11    | 7      | 1.57       | 1.57       | 0.3398124 | 6.9179×10^-7  | 2.452318×10^-5 | 25.27541 | 6.429105 | 2.248651×10^10 |
| 12    | 7      | 1.43       | 1.86       | 0.3329011 | 7.1184×10^-7  | 2.561732×10^-5 | 25.26134 | 6.435227 | 2.244879×10^10 |
| 13    | 7      | 2.29       | 2.29       | 0.3184553 | 9.8437×10^-7  | 3.124551×10^-5 | 25.13428 | 6.493624 | 2.258892×10^10 |
| 14    | 7      | 2.43       | 2.0        | 0.3297752 | 8.9553×10^-7  | 2.972186×10^-5 | 25.15267 | 6.481303 | 2.257151×10^10 |
| 15    | 7      | 2.71       | 2.14       | 0.3362088 | 9.5112×10^-7  | 3.184227×10^-5 | 25.16792 | 6.472815 | 2.255092×10^10 |
| 16    | 7      | 1.86       | 2.43       | 0.3221995 | 1.0234×10^-6  | 3.216713×10^-5 | 25.08916 | 6.487659 | 2.259931×10^10 |
| 17    | 7      | 2.57       | 2.57       | 0.3158822 | 1.1529×10^-6  | 3.351224×10^-5 | 25.03341 | 6.515021 | 2.263441×10^10 |
| 18    | 7      | 2.14       | 2.43       | 0.3284406 | 1.0712×10^-6  | 3.278456×10^-5 | 25.12186 | 6.499385 | 2.260412×10^10 |
| 19    | 7      | 2.29       | 2.71       | 0.3199021 | 1.1875×10^-6  | 3.412852×10^-5 | 25.04677 | 6.509826 | 2.262972×10^10 |
| 20    | 7      | 2.71       | 2.86       | 0.3171189 | 1.2042×10^-6  | 3.458891×10^-5 | 25.02815 | 6.518392 | 2.264185×10^10 |

---

## 3 Design and Simulation of a Bandgap Reference Circuit Using Xschem and Ngspice

The below photo is taken as the reference circuit for designing the Bandgap reference.

<img width="818" height="519" alt="Screenshot 2025-09-25 002310" src="https://github.com/user-attachments/assets/8c94dd5e-594b-4256-bc21-81022bf7fee3" />

## 3.1 Design using Xschem

![WhatsApp Image 2025-09-25 at 12 20 16 AM](https://github.com/user-attachments/assets/fa7564b7-7c51-40b5-82fe-cd0996e89608)

<details> <summary> <b>SPICE Deck bgr_dc_spice:</b> </summary>
	
```	
** sch_path: /home/vsduser/Desktop/asap_7nm_Xschem/bandgapcktfinal.sch
**.subckt bandgapcktfinal
Xpfet1 net3 net1 VDD net12 asap_7nm_pfet l=7e-009 nfin=14
Xpfet2 net2 net1 VDD net13 asap_7nm_pfet l=7e-009 nfin=14
Xpfet3 Vref net2 VDD net14 asap_7nm_pfet l=7e-009 nfin=14
Xpfet4 net4 net5 VDD net15 asap_7nm_pfet l=7e-009 nfin=14
Xpfet5 net9 net1 net4 net16 asap_7nm_pfet l=7e-009 nfin=14
Xpfet6 net6 net1 net5 net17 asap_7nm_pfet l=7e-009 nfin=14
Xnfet1 net10 net6 net3 net18 asap_7nm_nfet l=7e-009 nfin=14
Xnfet2 net7 net6 net2 net19 asap_7nm_nfet l=7e-009 nfin=14
Xnfet3 net8 net8 GND net20 asap_7nm_nfet l=7e-009 nfin=14
Xnfet4 net9 net9 net8 net21 asap_7nm_nfet l=7e-009 nfin=14
Xnfet5 net10 net10 GND net22 asap_7nm_nfet l=7e-009 nfin=14
R1 net7 net11 1k m=1
Xnfet6 net11 net11 GND net23 asap_7nm_nfet l=7e-009 nfin=14
R2 Vref VCTAT 1k m=1
Xnfet7 VCTAT VCTAT GND net24 asap_7nm_nfet l=7e-009 nfin=14
Xnfet8 net11 net11 GND net25 asap_7nm_nfet l=7e-009 nfin=14
Xnfet9 net11 net11 GND net26 asap_7nm_nfet l=7e-009 nfin=14
Xnfet10 net11 net11 GND net27 asap_7nm_nfet l=7e-009 nfin=14
V2 VDD GND 0.7
**** begin user architecture code


.dc temp -45 125 5
.control
run
plot v(Vref)
plot v(Vctat)
.endc


**** end user architecture code
**.ends
.GLOBAL VDD
.GLOBAL GND
**** begin user architecture code

.subckt asap_7nm_pfet S G D B l=7e-009 nfin=14
	npmos_finfet S G D B BSIMCMG_osdi_P l=7e-009 nfin=14
.ends asap_7nm_pfet

.model BSIMCMG_osdi_P BSIMCMG_va (
+ TYPE = 0

************************************************************
*                         general                          *
************************************************************
+version = 107             bulkmod = 1               igcmod  = 1               igbmod  = 0
+gidlmod = 1               iimod   = 0               geomod  = 1               rdsmod  = 0
+rgatemod= 0               rgeomod = 0               shmod   = 0               nqsmod  = 0
+coremod = 0               cgeomod = 0               capmod  = 0               tnom    = 25
+eot     = 1e-009          eotbox  = 1.4e-007        eotacc  = 3e-010          tfin    = 6.5e-009
+toxp    = 2.1e-009        nbody   = 1e+022          phig    = 4.9278          epsrox  = 3.9
+epsrsub = 11.9            easub   = 4.05            ni0sub  = 1.1e+016        bg0sub  = 1.17
+nc0sub  = 2.86e+025       nsd     = 2e+026          ngate   = 0               nseg    = 5
+l       = 2.1e-008        xl      = 1e-009          lint    = -2.5e-009       dlc     = 0
+dlbin   = 0               hfin    = 3.2e-008        deltaw  = 0               deltawcv= 0
+sdterm  = 0               epsrsp  = 3.9             nfin    = 1
+toxg    = 1.8e-009
************************************************************
*                            dc                            *
************************************************************
+cit     = 0               cdsc    = 0.003469        cdscd   = 0.001486        dvt0    = 0.05
+dvt1    = 0.36            phin    = 0.05            eta0    = 0.094           dsub    = 0.24
+k1rsce  = 0               lpe0    = 0               dvtshift= 0               qmfactor= 0
+etaqm   = 0.54            qm0     = 2.183e-012      pqm     = 0.66            u0      = 0.0237
+etamob  = 4               up      = 0               ua      = 1.133           eu      = 0.05
+ud      = 0.0105          ucs     = 0.2672          rdswmin = 0               rdsw    = 200
+wr      = 1               rswmin  = 0               rdwmin  = 0               rshs    = 0
+rshd    = 0               vsat    = 60000           deltavsat= 0.17            ksativ  = 1.592
+mexp    = 2.491           ptwg    = 25              pclm    = 0.01            pclmg   = 1
+pdibl1  = 800             pdibl2  = 0.005704        drout   = 4.97            pvag    = 200
+fpitch  = 2.7e-008        rth0    = 0.15            cth0    = 1.243e-006      wth0    = 2.6e-007
+lcdscd  = 0               lcdscdr = 0               lrdsw   = 1.3             lvsat   = 1441
************************************************************
*                         leakage                          *
************************************************************
+aigc    = 0.007           bigc    = 0.0015          cigc    = 1               dlcigs  = 5e-009
+dlcigd  = 5e-009          aigs    = 0.006           aigd    = 0.006           bigs    = 0.001944
+bigd    = 0.001944        cigs    = 1               cigd    = 1               poxedge = 1.152
+agidl   = 2e-012          agisl   = 2e-012          bgidl   = 1.5e+008        bgisl   = 1.5e+008
+egidl   = 1.142           egisl   = 1.142
************************************************************
*                            rf                            *
************************************************************
************************************************************
*                         junction                         *
************************************************************
************************************************************
*                       capacitance                        *
************************************************************
+cfs     = 0               cfd     = 0               cgso    = 1.6e-010        cgdo    = 1.6e-010
+cgsl    = 0               cgdl    = 0               ckappas = 0.6             ckappad = 0.6
+cgbo    = 0               cgbl    = 0
************************************************************
*                       temperature                        *
************************************************************
+tbgasub = 0.000473        tbgbsub = 636             kt1     = 0               kt1l    = 0
+ute     = -1.2            utl     = 0               ua1     = 0.001032        ud1     = 0
+ucste   = -0.004775       at      = 0.001           ptwgt   = 0.004           tmexp   = 0
+prt     = 0               tgidl   = -0.007          igt     = 2.5
************************************************************
*                          noise                           *
************************************************************
**)
.control
pre_osdi /home/vsduser/Desktop/asap_7nm_Xschem/bsimcmg.osdi
.endc



.subckt asap_7nm_nfet S G D B l=7e-009 nfin=14
	nnmos_finfet S G D B BSIMCMG_osdi_N l=7e-009 nfin=14
.ends asap_7nm_nfet

.model BSIMCMG_osdi_N BSIMCMG_va (
+ TYPE = 1
************************************************************
*                         general                          *
************************************************************
+version = 107             bulkmod = 1               igcmod  = 1               igbmod  = 0
+gidlmod = 1               iimod   = 0               geomod  = 1               rdsmod  = 0
+rgatemod= 0               rgeomod = 0               shmod   = 0               nqsmod  = 0
+coremod = 0               cgeomod = 0               capmod  = 0               tnom    = 25
+eot     = 1e-009          eotbox  = 1.4e-007        eotacc  = 1e-010          tfin    = 6.5e-009
+toxp    = 2.1e-009        nbody   = 1e+022          phig    = 4.2466          epsrox  = 3.9
+epsrsub = 11.9            easub   = 4.05            ni0sub  = 1.1e+016        bg0sub  = 1.17
+nc0sub  = 2.86e+025       nsd     = 2e+026          ngate   = 0               nseg    = 5
+l       = 2.1e-008        xl      = 1e-009          lint    = -2e-009         dlc     = 0
+dlbin   = 0               hfin    = 3.2e-008        deltaw  = 0               deltawcv= 0
+sdterm  = 0               epsrsp  = 3.9             nfin    = 1
+toxg    = 1.80e-009
************************************************************
*                            dc                            *
************************************************************
+cit     = 0               cdsc    = 0.01            cdscd   = 0.01            dvt0    = 0.05
+dvt1    = 0.47            phin    = 0.05            eta0    = 0.07            dsub    = 0.35
+k1rsce  = 0               lpe0    = 0               dvtshift= 0               qmfactor= 2.5
+etaqm   = 0.54            qm0     = 0.001           pqm     = 0.66            u0      = 0.0303
+etamob  = 2               up      = 0               ua      = 0.55            eu      = 1.2
+ud      = 0               ucs     = 1               rdswmin = 0               rdsw    = 200
+wr      = 1               rswmin  = 0               rdwmin  = 0               rshs    = 0
+rshd    = 0               vsat    = 70000           deltavsat= 0.2             ksativ  = 2
+mexp    = 4               ptwg    = 30              pclm    = 0.05            pclmg   = 0
+pdibl1  = 0               pdibl2  = 0.002           drout   = 1               pvag    = 0
+fpitch  = 2.7e-008        rth0    = 0.225           cth0    = 1.243e-006      wth0    = 2.6e-007
+lcdscd  = 5e-005          lcdscdr = 5e-005          lrdsw   = 0.2             lvsat   = 0
************************************************************
*                         leakage                          *
************************************************************
+aigc    = 0.014           bigc    = 0.005           cigc    = 0.25            dlcigs  = 1e-009
+dlcigd  = 1e-009          aigs    = 0.0115          aigd    = 0.0115          bigs    = 0.00332
+bigd    = 0.00332         cigs    = 0.35            cigd    = 0.35            poxedge = 1.1
+agidl   = 1e-012          agisl   = 1e-012          bgidl   = 10000000        bgisl   = 10000000
+egidl   = 0.35            egisl   = 0.35
************************************************************
*                            rf                            *
************************************************************
************************************************************
*                         junction                         *
************************************************************
************************************************************
*                       capacitance                        *
************************************************************
+cfs     = 0               cfd     = 0               cgso    = 1.6e-010        cgdo    = 1.6e-010
+cgsl    = 0               cgdl    = 0               ckappas = 0.6             ckappad = 0.6
+cgbo    = 0               cgbl    = 0
************************************************************
*                       temperature                        *
************************************************************
+tbgasub = 0.000473        tbgbsub = 636             kt1     = 0               kt1l    = 0
+ute     = -0.7            utl     = 0               ua1     = 0.001032        ud1     = 0
+ucste   = -0.004775       at      = 0.001           ptwgt   = 0.004           tmexp   = 0
+prt     = 0               tgidl   = -0.007          igt     = 2.5
************************************************************
*                          noise                           *
************************************************************
**)
.control
pre_osdi /home/vsduser/Desktop/asap_7nm_Xschem/bsimcmg.osdi
.endc


**** end user architecture code
.end


```bash
name=s1 only_toplevel=false value="
.dc temp -45 150 5
.control
pre_osdi /home/vsduser/Desktop/asap_7nm_Xschem/bsimcmg.osdi
run
plot v(Vref) v(Vctat)
plot v(Vref)-v(Vctat)
plot v(Vctat)
plot v(Vref)
let temp_coeff = deriv(v(Vref))/1.24
plot temp_coeff
plot net9/30k Vref/33.33k Vctat/33.33k
plot abs(v2#branch)
.endc
```
</details>


<img width="952" height="807" alt="Screenshot 2025-09-25 002904" src="https://github.com/user-attachments/assets/54a7c589-9ad8-4987-a750-448123516f7d" />





<img width="957" height="789" alt="Screenshot 2025-09-25 002915" src="https://github.com/user-attachments/assets/58100908-b046-4e46-91a8-faf94aedb3a3" />


BGRef Characterization Table

| S.No. | VDD (V) | Temp (°C) | Vref (V) | Line Reg. (mV/V) | Startup Time (ns) |
|-------|---------|-----------|----------|------------------|-------------------|
| 1     | 0.8     | 27        | 0.6615   | 827.4            | 55210.12          |
| 2     | 0.9     | 27        | 0.7482   | 828.55           | 51123.45          |
| 3     | 1.0     | 27        | 0.8308   | 829.1            | 47985.76          |
| 4     | 1.0     | -40       | 0.8399   | 837.65           | 75592.84          |
| 5     | 1.0     | 125       | 0.8169   | 816.2            | 29678.32          |

Conclusion

In this workshop, we explored the performance evaluation of 7 nm FinFET devices using the ASAP7 PDK. The sessions guided us through designing and simulating a Bandgap Reference Circuit with PFETs and NFETs in Xschem. We practiced generating SPICE netlists, running analyses in ngspice, and interpreting results. Key parameters such as startup behavior and reference voltage stability of the bandgap reference were investigated. Overall, the workshop strengthened both our understanding of advanced-node device modeling and our ability to carry out credible circuit analysis.

---


















