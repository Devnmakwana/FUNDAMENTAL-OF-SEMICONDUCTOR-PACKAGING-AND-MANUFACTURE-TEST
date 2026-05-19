# MODULE 3: FUNDAMENTALS OF SEMICONDUCTOR PACKAGING MATERIALS, QUALITY & RELIABILITY

---

### Day 1: Package Materials Part-1 
**Overview of IC Package Materials**
The primary elements constructing an IC package include Die Attach Film, Solder Balls, Epoxy Mold Compound (EMC), Bonding Wire, Substrate, and Underfill.

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/1cc95b05-37f0-49ff-853e-746f4f39852b" />

**Types of Interconnects**
* **Wire Bond:** Attaches thin wires to electrically connect semiconductor chips. Mainly used in packages with lower I/O.
* **Tape Automated Bonding (TAB):** Places bare ICs directly onto a flexible polyimide film carrier. Commonly used for SIM Cards and Bank Cards.
* **Flip Chip:** ICs are mounted in a face-down manner using C4 Solder Bumps or Copper Pillars to form the interconnection. Used for packages requiring higher I/O.
* **Clip Attach:** Instead of thick wires, it connects the die and lead using a solid copper bridge with adhesive bonding or soldering. Best for High Power Packages.

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/db5776d2-aa53-4bc5-9de7-8ed174ed9653" />


**Epoxy Mold Compound (EMC)**
EMC is a thermo-setting material (melts and hardens on heating via a cross-link reaction). It is irreversible and cannot be re-shaped. It protects the chip from mechanical shock, vibration, moisture, magnetism, high frequency, and harmful rays. 
* **Key Ingredients:** Main resin (Epoxy resin), Hardener (Phenol resin), Cure promoter/Catalyst (Phosphorus or Amine), Filler (Fused silica), Coupling agent (Silane), Releasing agent (Ester wax), and Flame retardant (Bromic epoxy resin).

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/1a2e904b-2a18-4ad9-998c-6df359e3c8a0" />

---

### Day 2: Package Materials Part-2
**Substrates Overview**
The substrate serves as the base support for the IC die and connects the die to the printed circuit board (PCB) through layout routing.

**Types of Substrates**
1.  **Ceramic Substrates:** Used for high-reliability products (military/space) and RF applications. They are used for hermetic packages to prevent gases/liquids from entering. They have a high dielectric constant and their Coefficient of Thermal Expansion (CTE) closely matches the silicon die.
2.  **Organic Substrates:** Cost-effective alternatives utilizing PCB manufacturing tech (e.g., Laminate BT, Tape Polyimide, Buildup). They feature lower dielectric constants, and their CTE matches the PCB.
3.  **Lead Frame:** Copper-based strips stamped/etched into circuit patterns. Exclusively used for wire-bonded dies, with a CTE suitable for direct assembly to the PCB.

**Organic Substrate Manufacturing Process**
1. **Core Baking**: Preparing raw materials.
2. **Half Etching**: Etching off the Cu surface to reduce thickness.
3. **Drill**: Creating holes to connect top and bottom layers.
4. **Cu Plating**: Electrically connecting the layers.
5. **Patterning**: Forming the circuit based on design.
6. **Solder Mask**: Applying organic photo ink to prevent Cu oxidation.
7. **Ni/Au Plating**: Creating bond fingers for wire bonding.
8. **Routing & Rinsing**: Cutting the panel to size and cleaning with DI water.

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/28dae38f-89b7-40e9-86ae-c375cc8b8f43" />


---

### Day 3: Package Materials Part-3
**What is a Solder Ball?**
Solder balls are the most common materials used to electrically interconnect PCBs and chip packages. They are created through sequential flow/quench or reflow processes. 

**Lead vs. Lead-Free Solder**
| Feature | Lead Solder Ball | Lead-Free Solder Ball |
| :--- | :--- | :--- |
| **Melting Point** | Lower | Higher |
| **Wettability** | Higher | Lower |
| **Eco-Friendly** | No | Yes |

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/4cb70973-1c49-4be5-93dc-932f298f1bcc" />
<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/72f19747-3b8f-4f9e-8baa-d585d927118a" />


**RoHS (Restriction of Hazardous Substances)**
Limits 10 specific substances in electronics. Strict thresholds are set for elements like Lead (Pb) < 1000 ppm, Mercury (Hg) < 1000 ppm, Cadmium (Cd) < 100 ppm, and Hexavalent chromium (Cr6+) < 1000 ppm. 

**Common Lead-Free Alloys**
* **SAC105:** 98.5% Tin (Sn), 1.0% Silver (Ag), 0.5% Copper (Cu)
* **SAC305:** 96.5% Tin (Sn), 3.0% Silver (Ag), 0.5% Copper (Cu)
* **SAC405:** 95.5% Tin (Sn), 4.0% Silver (Ag), 0.5% Copper (Cu)

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/7600e609-f980-4bea-843e-1ac0492f4f5a" />


---

### Day 4: Package Quality & Reliability Part-1
**Quality vs. Reliability**
* **Quality Failure:** Occurs during the manufacturing process (close to the ZERO time axis). Customers do not see these as they are rejected during final testing.
* **Reliability Failure:** Occurs during or after the customer's processing/usage.

**The Bathtub Curve (Failure Rate over Time)**
1.  **Infant Mortality (Phase 1):** Early life failures caused by gross manufacturing defects or lack of controls. Shows a *decreasing* failure rate.
2.  **Normal Life:** A period of useful life characterized by low, *constant* (random) failure rates.
3.  **Wear Out:** End-of-life failures showing an *increasing* failure rate. This is the stage that concerns both customers and manufacturers the most.

<img width="1865" height="1289" alt="image" src="https://github.com/user-attachments/assets/71b3d146-ee62-4ab0-9737-ad1ac80d0bae" />


---

### Day 5: Package Quality & Reliability Part-2
**Drivers of Package Reliability**
Package reliability ensures the product meets lifecycle performance. Key failure drivers include Hydro-mechanical stress (moisture swelling), Chemical stress (corrosion), Mechanical stress (drop/shock), and Thermal-Mechanical stress.

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/da8ac87f-2acc-41a4-81d3-3e3d45734dd0" />

**Coefficient of Thermal Expansion (CTE) Mismatch**
When high temperatures are applied during processing, the mold compound expands more than the die. When the temperature decreases, the mold compound shrinks more than the die. This unequal expansion/shrinkage leads to heavy internal stresses, ultimately causing **delamination and cracks**.

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/c1be9848-f4ee-4f12-b5cf-5d31265e3809" />

**Standard Package Reliability Tests**
* **MST:** Identifies moisture sensitivity classification (L1, L2).
* **Preconditioning (L3 Acc):** Simulates board assembly (e.g., IR/Convection Reflow) on moisturized packages prior to reliability testing.
* **Temperature Cycle (T/C):** 500 cycles to evaluate resistance to mechanical stresses from alternating temperature extremes.
* **High Temperature Storage (HTS):** Evaluates thermal failure mechanisms (e.g., at 150°C for 504 hours).

---

### Day 6: Package Quality & Reliability Part-3
**Highly Accelerated Stress Test (HAST)**
Evaluates moisture resistance in non-hermetic packages under severe conditions ($130^{\circ}C$, 85% RH, 19.5 psig) while applying an electrical bias. The bias creates an electrolytic cell that accelerates moisture and ionic penetration, eventually leading to metal corrosion and leakage. 
*Note: Not recommended for assembly packages with a Tg of less than $130^{\circ}C$ to avoid uncharacteristic failures.*

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/2993a4d0-6c16-4584-909a-4f004ef9fa98" />

**High Temperature Storage Life (HTSL / SLT)**
Stores devices at a continuous $+150^{\circ}C$ without electrical stress. It specifically tests bond integrity. Typical failures caught here include Kirkendall voiding (intermetallic formation), oxidation, and degradation of Au/Al bonding.

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/62d63032-5b86-4a57-9a18-41748abcb880" />

**Lead Integrity & Solderability Tests**
* **Lead Integrity:** Tests package robustness via tension (straight pull), bending stress, lead fatigue (8oz, 90-degree 3X bends), and lead torque.
* **Solderability:** Ensures solder can properly wet to the terminal of the package to survive board mounting.

---

### Day 7: Design For Reliability (DfR)
**DfR Methodology**
A multidisciplinary approach that brings together design, simulation, and material science. It relies heavily on understanding Material Properties (Young's modulus, Poisson ratio, Yield stress, CTE), utilizing Constitutive Models (Elastic, Plastic, Viscoelastic, Creep), and conducting Finite Element (FE) modeling for structural simulation.

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/7c1e64aa-4664-4679-889e-8548ec698896" />

**Solder Joint Reliability (SJR)**
The ability of a product's solder joints (which act as mechanical supports, electrical interconnects, and thermal dispersion paths) to function without exceeding acceptable failure levels.

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/b6445bac-4dd8-45ce-8087-fee3351fe9a7" />

**Assessing SJR**
Best done early in the New Product Introduction (NPI) stage using a combination of **Accelerated Stress Testing (AST)** (like Temperature Cycling) and **Finite Element Analysis (FEA)** to predict lifecycle and reduce the need for physical test vehicles.

**Typical Solder Joint Failure Modes**
1.  **Pad Lift:** Driven by severe overstress or aging degradation of adhesion.
2.  **IMC (Intermetallic Compound) Crack:** Brittle failure due to overstress, or micro-void formation from aging.
3.  **Bulk Solder Crack:** Occurs due to creep-fatigue under continuous cyclic loading.

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/96815278-f36d-479e-beb5-b135af718b91" />
