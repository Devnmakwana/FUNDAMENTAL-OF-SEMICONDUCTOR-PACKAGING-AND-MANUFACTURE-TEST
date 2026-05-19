# Module 5: Complete Guide To Industrial Quality In Atmp

This module covers Industrial Quality fundamentals used in semiconductor manufacturing, including Cost of Quality (CoQ), FMEA, control planning, measurement system validation, and statistical process control.  
It explains how quality is planned, measured, and controlled across ATMP production lines.  
It also introduces advanced manufacturing control systems like FDC and Run-to-Run (R2R) used in modern semiconductor manufacturing.

---

## Table of Contents

1. [Introduction to Industrial Quality](#1-introduction-to-industrial-quality)  
2. [Failure Mode and Effects Analysis (FMEA)](#2-failure-mode-and-effects-analysis-fmea)  
3. [Production Control Plans](#3-production-control-plans)  
4. [Calibration & Measurement Systems Analysis (MSA)](#4-calibration--measurement-systems-analysis-msa)  
5. [Statistical Process Control (SPC)](#5-statistical-process-control-spc)  
6. [Fault Detection Control (FDC) & Run-to-Run (R2R)](#6-fault-detection-control-fdc--run-to-run-r2r)

---

## 1: Introduction to Industrial Quality

### What is Quality?
[cite_start]According to Juran's Quality Handbook, quality means "fitness for purpose"[cite: 7]. [cite_start]To be fit for purpose, every good and service must have the right features to satisfy customer needs and must be delivered with few failures[cite: 9]. [cite_start]It must be effective (meeting customer requirements) and efficient (enabling superior business performance)[cite: 10]. 

<img width="2526" height="1734" alt="image" src="https://github.com/user-attachments/assets/0a5dbc3c-a411-43eb-a01a-062a12db2f89" />

[cite_start]If quality is ignored, minor problems can escalate, resulting in millions of dollars lost in revenue, warranty claims, legal actions, and damaged reputations[cite: 51].

### The Total Cost of Quality (CoQ)
[cite_start]To achieve high levels of quality, organizations must balance their investments to ensure the best outcome[cite: 146]. The mathematical framework is:
[cite_start]$CoQ = CoPQ + CoGQ$ [cite: 145]

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/a0998441-a674-4678-ae43-49aec7abb084" />

**1. [cite_start]Cost of Poor Quality (CoPQ):** $CoPQ = CoIF + CoEF$ [cite: 145]
* **Cost of Internal Failure (CoIF):** Occurs before delivery (e.g., reprocessing, rework, scrap)[cite: 151, 153].
* [cite_start]**Cost of External Failure (CoEF):** Occurs after delivery (e.g., warranty claims, recalls, lawsuits)[cite: 157, 160, 161, 162].

**2. [cite_start]Cost of Good Quality (CoGQ):** $CoGQ = CoA + CoP$ [cite: 145]
* **Cost of Appraisal (CoA):** Measuring, evaluating, or auditing products (e.g., incoming inspection, inline measurements)[cite: 167, 169, 170].
* [cite_start]**Cost of Prevention (CoP):** Minimizing failure and appraisal costs (e.g., quality planning, training, FMEA)[cite: 174, 176].

[cite_start]*Rule of Thumb:* $1 spent on Appraisal and Prevention Costs equals $10 saved on Internal and External Failure Costs[cite: 514].

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/48115a24-e2c3-434c-b060-81b7194823da" />

---

## 2: Failure Mode and Effects Analysis (FMEA)

[cite_start]FMEA is a systematic, qualitative, team-oriented analytical method designed to identify potential technical risks of failure, their effects, and their causes[cite: 244]. [cite_start]It focuses on *proactive* risk mitigation rather than reactive troubleshooting[cite: 238].

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/0c8a540d-a4bd-42d7-8dd2-5563b8a696cb" />

### DFMEA vs. PFMEA
* **Design FMEA (DFMEA):** Focused on the product and design intent[cite: 283, 286]. *Rule of thumb: Assume that the manufacturing process does not exist*[cite: 270].
* [cite_start]**Process FMEA (PFMEA):** Focused on the manufacturing and assembly process[cite: 288]. [cite_start]*Rule of thumb: Assume that the design is perfect*[cite: 275].

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/bab06957-908c-4c81-9666-216440acf366" />

### The 7-Step Approach
[cite_start]The AIAG-VDA FMEA process follows seven steps[cite: 361, 362]:
1.  [cite_start]Planning and Preparation [cite: 362]
2.  [cite_start]Structure Analysis [cite: 362]
3.  [cite_start]Function Analysis [cite: 362]
4.  [cite_start]Failure Analysis [cite: 362]
5.  [cite_start]Risk Analysis [cite: 362]
6.  [cite_start]Optimization [cite: 362]
7.  [cite_start]Results Documentation [cite: 362]

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/c5d5035c-5d3e-441b-91da-bae7b4119b84" />

### Risk Scoring (SOD)
[cite_start]Risks are ranked on a scale of 1-10[cite: 336]:
* [cite_start]**Severity (S):** Consequence of the failure (e.g., 10 = Safety risk, 1 = No effect)[cite: 341].
* **Occurrence (O):** Probability of the failure cause (e.g., 10 = No preventive controls, 1 = Error proofed)[cite: 342].
* [cite_start]**Detection (D):** Ability to detect the failure (e.g., 10 = No detection method, 1 = Error proofed)[cite: 344].

[cite_start]These scores determine the **Action Priority (AP)** (High, Medium, or Low), which dictates whether action *must*, *should*, or *could* be taken[cite: 355].

---

## 3: Production Control Plans

[cite_start]The Control Plan is the "operational expression" of the FMEA[cite: 383]. [cite_start]It is a written description of the control systems and parameters needed to minimize product and process variation[cite: 403]. [cite_start]Actions and controls identified in the FMEA flow directly into the Control Plan[cite: 556].

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/a39da21a-3b4d-499f-897b-bf54abd902b3" />

### Types of Control Plans
1.  [cite_start]**Prototype:** Dimensional measurements and tests occurring during the prototype build[cite: 524].
2.  [cite_start]**Pre-Launch:** Developed during process design and validation[cite: 526].
3.  [cite_start]**Safe-Launch:** A period of enhanced containment and increased inspection frequency at the start of production[cite: 527, 529].
4.  [cite_start]**Production:** Used for controlling the process during volume manufacturing runs[cite: 531, 533].

---

## 4: Calibration & Measurement Systems Analysis (MSA)

### Calibration
[cite_start]Calibration involves comparing an unknown measurement device (Device-under-Test) against a known standard under specified conditions[cite: 611, 614, 617].
* **Traceability:** This is the unbroken chain of calibration and associated uncertainty back to a National Standard[cite: 641].
* [cite_start]**Maximum Permissible Error (MPE):** For devices determining product disposition, the MPE should be the OEM spec or 25% of the tightest application specification, whichever is tighter[cite: 693].

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/22d7fc9d-8c65-46ed-b780-5083a5fa91a5" />

### Measurement Systems Analysis (MSA)
[cite_start]MSA determines if the measurement system can detect "real" differences in a process[cite: 717]. Measurement errors fall into two categories:
* **Location Variation:** Accuracy, Bias, Stability, and Linearity[cite: 721, 722, 723].
* [cite_start]**Width Variation:** Precision, Repeatability, and Reproducibility (GR&R)[cite: 724, 725, 726].

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/42041cc5-dc03-4cce-92ef-22e85826dac9" />

---

## 5: Statistical Process Control (SPC)

[cite_start]SPC is a statistical method to control and monitor the quality of a production line, ensuring it operates at its full potential with minimum waste[cite: 734, 736].

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/a02078a9-f408-42d5-8c9f-a55e40fea779" />

### Types of Variation
* **Common Cause Variation:** Inherent noise in a process due to random effects; it is predictable and stays within statistical limits[cite: 872].
* [cite_start]**Special Cause Variation:** Unexpected glitches or assignable causes that significantly affect a process, making it unstable[cite: 873, 874].

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/525147e4-a8d5-4520-8aad-b62fc5f8ed01" />

### Control Charts & Capability
[cite_start]Control charts track observations over time against a Center Line, Upper Control Limit (UCL), and Lower Control Limit (LCL)[cite: 771]. Standard deviation is defined as:
[cite_start]$s_{x}=\sqrt{\frac{\sum_{i=1}^{n}(x_{i}-\overline{x})^{2}}{n-1}}$ [cite: 846]

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/9589c330-4b7e-4d5e-8bdf-5a93721d00c0" />

[cite_start]Process capability calculates how well the process output meets customer specifications[cite: 915]. 
* Capability Potential ($C_p$):
    [cite_start]$C_p = \frac{USL - LSL}{6\sigma}$ [cite: 917]
* Process Capability Index ($C_{pk}$):
    $C_{pk} = \min(\frac{USL - \bar{x}}{3\sigma}, \frac{\bar{x} - LSL}{3\sigma})$ [cite: 917]

A process is considered "good" when $C_p > 1.33$[cite: 917].

---

## 6: Fault Detection Control (FDC) & Run-to-Run (R2R)

To meet the demands of leading-edge manufacturing, Advanced Process Control (APC) replaces traditional manual intervention with real-time process control[cite: 930].

* [cite_start]**FDC (Fault Detection & Classification):** Collects real-time trace data from equipment sensors (e.g., temperature, pressure, vibration) to monitor health and detect abnormalities[cite: 937, 939, 940, 943]. [cite_start]When a fault is detected, it triggers an Out-of-Control-Plan (OCAP)[cite: 948].
* **R2R (Run-to-Run Control):** Modifies the process recipe between machine runs using metrology feedback[cite: 1054]. This minimizes process drift, reduces variability, and ensures a stable output[cite: 1054, 1101].

<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/988b9854-5cc4-4280-a280-93d261f54971" />

---

