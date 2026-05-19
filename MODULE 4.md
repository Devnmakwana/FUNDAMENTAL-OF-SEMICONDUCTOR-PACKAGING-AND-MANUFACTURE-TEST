# MODULE 4: FUNDAMENTALS OF IC PACKAGE FAILURE ANALYSIS

## Table of Contents
1. [Day 1: Introduction to Failure Analysis & Basic Flow](#day-1-introduction-to-failure-analysis--basic-flow)
2. [Day 2: Electrical Data Analysis & EFA](#day-2-electrical-data-analysis--efa)
3. [Day 3: Visual Inspection (OM, SAM, X-Ray)](#day-3-visual-inspection)
4. [Day 4: Fault Isolation Techniques - I (Thermography)](#day-4-fault-isolation-techniques---i)
5. [Day 5: Fault Isolation Techniques - II (Emission & SEM Probing)](#day-5-fault-isolation-techniques---ii)
6. [Day 6: Physical/Destructive Failure Analysis - I](#day-6-destructive-failure-analysis---i)
7. [Day 7: Physical/Destructive Failure Analysis - II](#day-7-destructive-failure-analysis---ii)
8. [Day 8: Case Studies](#day-8-case-studies)

---

### Day 1: Introduction to Failure Analysis & Basic Flow
**Overview of Failure Analysis (FA)**
Failure analysis determines how or why a semiconductor device failed (deviating from its electrical, visual, or mechanical requirements). Identifying the root cause is critical for implementing corrective actions and avoiding future recurrences.

**Non-Destructive vs. Destructive Analysis**
* **Non-Destructive:** Curve tracing, Optical Microscopy, Scanning Acoustic Microscopy (SAM), 2D/3D X-ray, IR Thermography.
* **Destructive:** Irreversible processes performed only after non-destructive steps. Includes Decapsulation, Cross-section/Grinding, Focused Ion Beam (FIB), and Dye and Pry.

**Standard FA Process Flow**
1. Electrical Test Verification (ATE to Bench)
2. Electrical Failure Analysis (EFA) & Curve Trace
3. Non-Destructive FI (Fault Isolation)
4. Physical/Destructive FA
5. Identify Mechanism and Generate Report

<img width="2520" height="1398" alt="Screenshot 2026-05-19 181923" src="https://github.com/user-attachments/assets/a27e9968-d3c6-4ed4-a2bd-9e973eede05b" />


---

### Day 2: Electrical Data Analysis & EFA
**Electrical Data Analysis (EDA)**
Every IC is tested at wafer and package levels. Analyzing this data (checking Upper/Lower Cut-off Limits - UCL/LCL) reveals outlier parts and early insights into the failure distribution.

**Electrical Failure Analysis (EFA)**
EFA is performed on the bench to verify the fault and classify the failure mode (e.g., Short, Open, Leakage, Functional). 
* **Curve Tracing:** A foundational tool used to generate I-V (Current-Voltage) curves. Comparing a failed pin's I-V curve to a "Golden" (known good) device helps determine if a pin is shorted to ground/power, open, or leaking.

<img width="2525" height="1420" alt="image" src="https://github.com/user-attachments/assets/98d41793-ad40-4e99-81be-3b0b3a2eef68" />


---

### Day 3: Visual Inspection
**1. Optical Microscopy (OM)**
Uses visible light and lenses to inspect the external package for obvious physical damage (cracks, chip-outs, discoloration).

**2. Scanning Acoustic Microscopy (SAM / C-SAM)**
Uses ultrasonic waves to detect changes in acoustic impedance. Excellent for finding internal delamination (separation of layers), voids, or cracks at interfaces (e.g., Die-to-Mold Compound, Die Attach).

<img width="2526" height="1420" alt="image" src="https://github.com/user-attachments/assets/de6ace9f-0cb6-4561-a139-f4985d667b74" />


**3. 2D / 3D X-Ray**
Uses an electron beam to excite a target into producing X-rays. X-rays pass through the package, allowing inspection of internal, high-density structures. 
* **Target Defects:** Broken/lifted wire bonds, missing solder balls, non-wet solder joints, and foreign material bridges.

<img width="2527" height="1410" alt="image" src="https://github.com/user-attachments/assets/ef4611dd-7ffa-48bb-bf51-d40ce1521189" />
<img width="2528" height="1420" alt="image" src="https://github.com/user-attachments/assets/24618bcf-6b78-45f6-bc5d-3fede931b6b7" />


---

### Day 4: Fault Isolation Techniques - I
**IR Thermography (Hotspot Detection)**
When a short or leakage is present, it generates abnormal heat. Elite IR Thermography uses InSb detectors to find absolute temperature hotspots (detecting where the short is located).

**Lock-In Thermography**
Synchronizes the camera acquisition rate with a pulsating electrical excitation of the circuit. 
* Provides significantly higher Signal-to-Noise (S/N) ratio.
* The Phase Image allows estimation of the **Depth (Z-axis)** of the defect.
* The Amplitude Image estimates the **X-Y location** of the defect.

<img width="2524" height="1421" alt="image" src="https://github.com/user-attachments/assets/777903d9-3793-41e6-950d-f1f42763bae0" />
<img width="2522" height="1419" alt="image" src="https://github.com/user-attachments/assets/4505092f-44bc-4e91-8b8c-bb596404dcce" />


---

### Day 5: Fault Isolation Techniques - II
**NIR Photon Emission**
Captures near-infrared (NIR) photon emissions generated from electron-hole pair recombination. Highly effective for detecting junction breakdowns, gate oxide defects, and latch-up events in the silicon die.

**Passive Voltage Contrast (PVC)**
Uses an SEM (Scanning Electron Microscope). Because of different charging effects, grounded structures appear bright (they have a discharge path), while isolated or floating structures appear dark. Great for finding opens in vias or contacts.

**SEM Probing FI Techniques:**
* **EBAC (Electron Beam Absorbed Current):** Detects breaks in buried metal lines.
* **EBIC (Electron Beam Induced Current):** Characterizes PN junctions.
* **EBIRCH (Electron Beam Induced Resistance Change):** Identifies resistive shorts or leakages.

<img width="2525" height="1419" alt="image" src="https://github.com/user-attachments/assets/702fef0f-5cc3-4aed-89d0-ed4a35644012" />
<img width="2526" height="1420" alt="image" src="https://github.com/user-attachments/assets/6883d013-e666-47ab-a0c8-41506d69cfa0" />


---

### Day 6: Destructive Failure Analysis - I
**Decapsulation (Decap)**
The chemical (acid) or laser removal of the Epoxy Mold Compound (EMC) to expose the top surface of the die and wire bonds for inspection (checking for EOS, ESD, or die surface damage).

**Cross Section (Grinding / Polishing)**
Mechanically sawing, grinding, polishing, and sometimes staining a sample until the specific plane of interest is exposed. 
* **Target Defects:** Substrate via cracks, solder ball non-wetting, copper migration, and exact Z-axis measurements.

<img width="2521" height="1420" alt="image" src="https://github.com/user-attachments/assets/9f268823-8357-47e7-82f0-acafe9fe191b" />


**Die Delayering**
Removing upper metallization/dielectric layers of a die using Plasma/RIE (Reactive Ion Etching) or wet chemicals to expose underlying wafer fab defects or Electrical Over-Stress (EOS) damage.

<img width="2523" height="1418" alt="image" src="https://github.com/user-attachments/assets/184c013b-7690-47a8-bbd8-c0ec4fef472c" />

---

### Day 7: Destructive Failure Analysis - II
**Dye and Pry**
A destructive mechanical technique used specifically to test for cracks in solder joints (often BGA to PCB). 
* **Process:** The sample is immersed in red dye, subjected to a vacuum, baked dry, and then mechanically pried off. 
* **Result:** If a crack was present before prying, the red dye will be visible on the separated fracture interfaces.

<img width="2522" height="1410" alt="image" src="https://github.com/user-attachments/assets/3214bac1-78b5-43bb-80fa-dcbe8337ae84" />


**Energy Dispersive X-Ray (EDX / EDS)**
Integrated with a Scanning Electron Microscope (SEM). The electron beam hits the sample, ejecting inner shell electrons. When outer shell electrons drop down to fill the vacancy, they emit X-rays characteristic of the specific element.
* **Application:** Identifies the exact elemental composition of foreign materials, contamination, or corrosion.

<img width="2517" height="1410" alt="image" src="https://github.com/user-attachments/assets/51f9e4d5-ccf7-4732-b665-ce309182bd46" />


---

### Day 8: Case Studies
**Putting It All Together**
Applying the FA flow to real-world scenarios:
1.  **Open Failure Flow:** Verified via Curve Trace $\rightarrow$ 3D X-Ray (check for broken wires) $\rightarrow$ C-SAM $\rightarrow$ Cross-section at the broken location.
2.  **Short/Leakage Failure Flow:** Verified via Curve Trace $\rightarrow$ IR Thermography (to find the hotspot) $\rightarrow$ Decap / Z-Grind $\rightarrow$ SEM/EDX to check for copper migration or foreign material shorts.

<img width="2524" height="1417" alt="image" src="https://github.com/user-attachments/assets/832bdb54-5164-42da-abc3-71f001773c11" />
