# FUNDAMENTAL-OF-SEMICONDUCTOR-PACKAGING-AND-MANUFACTURE-TEST

# Semiconductor Backend Manufacturing (ATMP) Masterclass

![Domain](https://img.shields.io/badge/Domain-VLSI%20%26%20ATMP-orange.svg)
![Status](https://img.shields.io/badge/Status-Module%201%20Completed-brightgreen.svg)

This repository contains the complete, unabridged documentation of the **Semiconductor Backend Manufacturing (Assembly & Test)** curriculum. This covers the entire Assembly, Testing, Marking, and Packaging (ATMP) flow. 

---

## Chapter 1 (Lecture 1): New Product Introduction (NPI) & Memory Packaging

### Overview of Semiconductor Systems
The semiconductor manufacturing flow transitions from a bare Wafer ➔ IC Package ➔ System. The key driving factors are Performance, Cost, Reliability, and Time to Market.

**Making IC Package - Process Steps:**
1. **Fab:** Chip Design ➔ Technology Development ➔ Fabrication
2. **Probe**
3. **Assembly (ATMP):** Die Preparation (Thinning, Dicing) ➔ Die attach ➔ Wirebond ➔ Encapsulation ➔ Laser Marking ➔ Solder Ball Attach ➔ Singulation
4. **Final Test:** Package Backend Test (Tester, Test Firmware, Test Program Debugging, Burn In, ATE Flow, FQMON, Aging)
5. **Materials & Qualification:** Package Materials, Reliability, Moisture Sensitivity Level (MSL), Temperature Humidity, Temperature Cycling, Thermal Shock, High Accelerated Stress Test.
6. **EFA & PFA (Failure Analysis):** Inspection, SI Failures, Etching, Dye & Pry.
7. **Quality & Process Control:** ESD, Industrial Quality, FMEA, Quality Control Plan, MSA/Calibration, Process Control, Fault Detection Control (FDC), Run to Run Control.

### What is IC Packaging?
The IC Packaging shields the semiconductor chip from external loads, moisture, physical damage and provides electrical contacts that deliver signals to the Printed Circuit Board (PCB).
* **Functions:** Signal distribution, Power distribution, Heat dissipation, Protection (Mechanical/Chemical/Electromagnetic).
* **Components:** Molding Compound (Protects DIE), DIE (Semiconducting material), Die Attach Film (For stacking dies), Substrate (Mechanical strength/signal routing), Wirebond (Interconnection), Solder Joint (Mechanical/Electrical connection).

### Evolution of Memory Packaging
* **<1980s to 1990s:** Protect & Connect Silicon (4 to 8 I/Os) ➔ Manufacturing Scale
* **2000s:** Form Factor, Performance (16 to 32 I/Os)
* **2005 - 2010:** Density, 3D System ➔ Density with Bandwidth, Package Level ECC (48 I/Os) ➔ Package Density, Security, Performance (96 I/Os)
* **Today & Future:** Density, Performance (200 I/Os) ➔ New Interface, System Level Collaboration (1000+ I/Os).

### Memory & Storage Package Configurations
1. **Ultra-High Bandwidth PKGs (Graphics, HBM):** High bandwidth memory DRAM cube connected with several thousand TSVs at < 40 um pitch.
2. **DRAM PKGS:** Performance DRAM memory. Single or dual die packages connected as flip-chip or wire bond & integrated on module system.
3. **Multichip PKGS (LPDRAM + NAND):** Low-power & mass-storage memory. Multiple (8+) wire bond die integrated into a single package.
4. **SSD Drives:** Large, complex board- or package-level system with several hundred components.

### NPI (New Product Introduction) Impact on Product Lifecycle
A focus on NPI minimizes investment, reduces time, improves revenue, and prolongs lifecycle.
* **Stages:** 1. Product Concept ➔ 2. Requirement Definition ➔ 3. Design & Assembly ➔ 4. Validation & Qualification ➔ 5. Low-Volume Manufacture ➔ Production.
* **DFMEA (Design Failure Mode and Effects Analysis):** Used during design to identify and mitigate potential failures (Risk Priority = Severity x Occurrence x Detection).

---

## Chapter 1 (Lecture 2): Introduction to Backend Assembly Processes

### Semiconductor Wafer to IC Package Flow
* **Incoming Wafer:** Si Wafer 300 mm, ~900 um thickness.
* **Substrate/Interposer:** Bond pads on 4 sides. 
* **Molded IC Packaging:** Assembled in entire substrate/strip form.

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/8a153567-38f9-4f7c-ab44-37aa53428350" />


### Why Memory Packaging is Challenging
Memory packages deal with die thicknesses ranging from 300 um down to 30um (Incoming wafer thickness is 800-900 um).
* Wafer Grinding: ~30-150 um.
* Wire Bond: ~400 wires at 15-18 um.
* Die Attach: 1D to 32D stacking.
* Mold: Powder Mold Compression (PMC).

### Assembly Process Flow
1. **Die Bank & Wafer Tape** ➔ **Wafer Thinning** ➔ **Wafer Mount** ➔ **Wafer Detape**
2. **Die Preparation:** Laser Groove ➔ Wafer Saw ➔ UV.
3. **Die Attach (and Cure):** Oven Cure.
4. **Plasma Treatment:** Plasma Clean 1.
5. **Wire Bond (Interconnect)**
6. **Plasma Treatment:** Plasma Clean 2.
7. **Encapsulation and Baking**
8. **Laser Scribe / Laser Mark**
9. **Solder Ball Attach:** Solder Flux printing ➔ Solder Ball Attach + Reflow.
10. **Singulation**
11. **Automated Visual Inspection (AVI) / Open Short (OS) Test**
12. **Electrical Test**

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/f127850f-2101-4608-9493-1e75f8a296d1" />


---

## Chapter 1 (Lecture 3): Die Preparation Step

### Die Prep Processing Comparison
| Feature | LGD (Laser Groove Dicing) | DBG (Dice Before Grind) | SDBG (Stealth Dice Before Grind) |
| :--- | :--- | :--- | :--- |
| **# Dicing step** | 2 | 1 | 1 |
| **Crack Generated** | Externally | Externally | Internally |
| **Dicing Quality - Sidewall** | Blade marking | Blade Marking | Smooth |
| **Dicing Quality - Die edge** | Have chipping | Have Chipping | Smooth |
| **Productivity/Yield** | Slow | Slow | Fast (2-5X) |
| **Die strength** | Low | Low | High (2-3X) |

*Die strength is approximately 2.2 times stronger in SDBG compared to LGD.*

### Materials Used in Die Prep
* **Direct Materials:** Die Attach Film (DAF) - interacts with die and becomes part of the package.
* **In-Direct Materials:** Coating materials, Cleaning water, Backgrind tape/Dicing tape, Grinding wheel, Dicing Blade.

### Characteristics of a Saw Blade
* **Blade Dicing:** Uses a high-speed blade to cut through scribe and silicon.
* **Laser Grooving:** Laser ablates majority of metals from scribe materials to expose Silicon to allow blade dicing. It prevents peeling defects that propagate into the active area.
* **Coolant:** RO water or DI water is used to remove debris, remove heat, and increase lubrication.

### Stealth Dicing before Grinding (SDBG)
An advanced, cleaner process where bulk Si is cracked internally to effectively separate dies.
* Crack is induced by focusing an IR light inside the bulk silicon.
* The localized heat raises the temperature, inducing nonlinear absorption, raising the localized temp up to 5~10K°C. This produces a Heat Affected Zone (HAZ) of 10um, causing rapid vaporization of silicon, inducing massive pressure build-up and a crack (SD Modified Layer).

---

## Chapter 1 (Lecture 4): Die Attach Process

### What is Die Attach?
The process of removing singulated dies from the wafer and attaching them to the interposer/substrate/Leadframe using an adhesive.

### Die Stacking Configurations
* **Direct Shingled Stack**
* **Reverse Shingle on Shingled Stack (RSOS)**
* **Same Size Die Stacking (Using FOW - Film Over Wire)**
* **Flip-flop Stack**
* **Hybrid Stack**

Factors influencing stack configuration: Die size, Package size, Die bond pad location, Signal integrity, Assembly process, Substrate design, Package warpage, Package reliability, and Cost.

### Types of Adhesives
1. **Epoxy Paste:** For Chip-on-board (COB), dispensed onto interposer before die bonding. Needs oven cure.
2. **Stencil Printed Paste:** For Board-on-chip (BOC).
3. **"LOC" (Lead-on-chip) Tape:** For TSOP packages; pre-taped on metal Leadframe. No oven cure needed.
4. **Die Attach Film (DAF):** For single/stacked Chip on Board. Taped on wafer backside. Needs oven cure.
5. **Film Over Wire (FOW) & Film Over Die (FOD):** Used for stacking dies over existing wirebonds or entire bottom dies.

### Key Die Attach Parameters
* **Mount/Bond Time:** Time held on die to interposer.
* **Mount/Bond Force:** Weight/Load exerted on die.
* **Mount/Bond Temperature:** Temperature applied during die attach.

### Process Control & Defects
* **Tape bubbling:** Root causes include overbaked leadframes, high mount temp, or high mount time.
* **Adhesive on die:** Mount force too high, planarity out, or viscosity too low.
* **Slant/Die Placement issues:** Pickup collet loose, vacuum malfunction, or bondhead malfunction.

---

## Chapter 1 (Lecture 5): Wirebond Assembly Process

### What is Wirebond?
Wirebond creates electrical interconnections between an integrated circuit and a substrate using a Capillary assisted Thermosonic Bonding process. Gold wire is primarily used due to its excellent electrical conductivity and corrosive resistance.

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/e400688a-4982-49d9-89ac-3e9d2ce4990f" />


### Wire Bonding Sequence
1. **Free Air Ball (FAB):** Formed by Flame off Electrode.
2. **1st Bond (Ball Bond):** Capillary applies force and ultrasonics to bond the FAB to the die pad.
3. **Looping:** Capillary moves to form the wire trajectory.
4. **2nd Bond (Stitch Bond):** Capillary bonds the wire to the substrate lead/pad.
5. **Wire Clamp:** Breaks the wire to restart the cycle.

### Loop Types
* Multi Stack Direct Cascade
* Multi Stack Direct Bonding
* Forward Cascade vs. Forward Compressed Loop

### Quality Checks
* **Ball Shear Test:** Checks adhesion between bond pad and bonded ball (Modes: Ball Lift, Ball Shear, Pad Metal Lift, Cratering).
* **Wire Pull / Stitch Pull:** Checks adhesion between pad, wire, and leadfinger (Modes: Break at Neck, Break at Stitch, Ball Lift, Stitch Lift).
* **Intermetallic Coverage (IMC):** Checking the growth of $Au_xAl_y$ intermetallic compounds (Kirkendall voids monitoring).

---

## Chapter 1 (Lecture 6): Flip Chip & Underfill Technology

### Flip Chip Process
The chip is mounted onto the substrate with the active side facing down. Cu pillar is widely used as the interconnection material.
* **Bonding Methods:** Mass Reflow (Heat convection), Thermal Compression Bond (TCB), Laser Assisted Bond (LAB).
* **Process Flow:** Boat Carrier Mount ➔ Pre-FC Substrate Bake ➔ Flip Chip Attach ➔ Mass Reflow ➔ Flux Cleaning ➔ Underfill ➔ Underfill Cure.

### What is Flux?
A chemically active formula that promotes wetting of a metal surface.
* Removes oxide from base metals ($Sn/Ag$ & Cu).
* Organic acid removes OSP (Organic Solderability Preservative) layer.
* Prevents re-oxidation during reflow.
* **Types:** Water soluble, Non-clean, Underfill-less (Epoxy flux).

### What is Underfill?
Thermo-setting encapsulant in liquid form dispensed between the die and substrate. Flows via capillary effect.
* **Function:** Acts as a buffer for mechanical stress caused by Coefficient of Thermal Expansion (CTE) mismatch between the silicon die and organic substrate. Protects bumps from cracking.
* **Defect Modes:** Voids due to dispense pattern, moisture absorption, or flux residue.

---

## Chapter 1 (Lecture 7): Encapsulation & Laser Marking

### Encapsulation Process
Enclosing the product in an Epoxy Mold Compound (EMC) to provide a moisture barrier, heat transfer, electrical insulation, and a medium for laser marking.

### Transfer Molding vs. Compression Molding
| Feature | Transfer Mold | Compression Mold |
| :--- | :--- | :--- |
| **Process Mechanism** | Compound transferred via cull and runner | Fix cavity configuration |
| **Advantages** | Free from pellet size requirement | Much less compound wastage; Good for wire sweep with thinner wires |
| **Disadvantages** | More compound usage; Prone to wire sweep | Expensive (release film ETFE required) |

*Common Mold Defects:* ECSM (Foreign material stuck), EVDS (Internal Voids), Wire Sweep (Unbalanced flow).

### Laser Marking
Marking the identity of the package:
1. **2DID:** Individual package identification.
2. **Pin 1:** Package Orientation.
3. **Lot Trace Code (LTC):** Lot level identification.
* **Control:** Laser mark readability and Laser Mark Depth (incorrect depth causes exposed wires/dies).

---

## Chapter 1 (Lecture 8): Solder Ball Attach & Reflow

### Ball Attach Process
Attaching solder balls permanently on the ball pads (NiAu or CuOSP) of the interposer using temperature reflow.
* **Solder Ball Types:** SAC302, SAC305, SAC405, SACN105, SACQ.
* **Flux:** Printed via pin-transfer to seal out air, remove oxidation, and hold pre-formed solder balls in place.

### Reflow Process & Warpage
* **Reflow Oven:** Provides heat via thermal convection using heated $N_2$ gas to prevent oxidation. 
* **Zones:** Pre-heat ➔ Soak ➔ Ramp up (Solder Melting) ➔ Dwell ➔ Cool down (Solder Solidification).
* **Warpage:** High temps ($250^\circ C$) cause die/substrate expansion mismatch. Creates **Convex (+)** (Crying shape) or **Concave (-)** (Smile shape) warpage.

### Post-Reflow
* **De-flux Cleaning:** Input ➔ Chemical Wash ➔ DI Water Wash ➔ DI Water Rinse ➔ Dry. Prevents corrosion of Cu patterns.
* **Defects:** Solder Crack, Non-wet, Double Ball, Bridging, Missing Ball.

---

## Chapter 1 (Lecture 9): Singulation

### Introduction to Singulation
Separating the BGA package into individual units from its strip/interposer form using ultra-thin diamond cutting blades.

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/2105d2f1-1f26-411d-adb8-f44228149eee" />


### Process Flow
1. **Loader:** Substrate orientation check.
2. **Vision Alignment:** Automatic strip geometry compensation.
3. **Singulator (Saw):** Upside-down sawing using Single Blade or Dual Spindle.
4. **Clean & Dry:** Top/bottom cleaning and air atomizing.
5. **Product Inspection:** 100% top/bottom inspection.
6. **Sorting Offload:** JEDEC tray compatible.

### Characteristics of a Saw Blade
* **Grit Size:** E.g., #2000 (Openings in Mesh per Square Inch).
* **Bond Types:** Resin, Metal, Vitrified, Electroplated. Contains chip pockets for whisking away particles and bringing in coolant.
* **Truing vs. Dressing:** Truing makes OD concentric with spindle center. Dressing exposes new diamond crystals to improve cut quality.

### Cut Quality Definitions
Defects monitored during singulation include:
* **Copper Smear**
* **Burr Height**
* **Package Chipping / Cracked Packages**
* **Damaged Balls** (Handler misalignment)

---
