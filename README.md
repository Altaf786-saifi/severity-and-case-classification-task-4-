# severity-and-case-classification-task-4-

## Overview
This repository contains the evaluation and classification of adverse drug reaction (ADR) cases based on **seriousness** and **expectedness** using standard pharmacovigilance guidelines, along with the setup methodology for creating structured case classification sheets.

---

## 1. Pharmacovigilance Guidelines & Definitions

### Seriousness Criteria
According to standard pharmacovigilance guidelines (ICH E2A), an adverse event or reaction is classified as **Serious** if it results in any of the following outcomes:
* Death
* A life-threatening condition
* Inpatient hospitalization or prolongation of existing hospitalization
* Persistent or significant disability or incapacity
* A congenital anomaly or birth defect
* Any other medically important condition that may jeopardize the patient or require medical/surgical intervention to prevent one of the outcomes above.

Events that do not meet any of these criteria are classified as **Non-Serious**.

### Expectedness Criteria
* **Expected:** The adverse reaction is consistent in nature, severity, and specificity with the established reference safety information (e.g., drug label, Package Insert, or Summary of Product Characteristics / SmPC).
* **Unexpected:** The adverse reaction is not listed in the current product labeling, or occurs at a greater severity or specificity than documented.

---

## 2. Case Classification & Severity Analysis Table

Below is the evaluation of the clinical cases provided in the task dataset:

| Case ID | Suspected Drug | Adverse Reaction | Seriousness | Expectedness | Clinical Impact & Justification |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **01** | Amoxicillin | Skin rash, itching | **Non-Serious** | **Expected** | Mild cutaneous hypersensitivity reaction. Listed in the SmPC for penicillin-class antibiotics and does not require hospitalization or pose a life threat. |
| **02** | Ibuprofen | Gastrointestinal bleeding requiring hospitalization | **Serious** | **Expected** | Classified as **Serious** because it required inpatient hospitalization. **Expected** because GI ulceration and bleeding are well-documented risks of NSAIDs on the product label. |
| **03** | Metformin | Lactic acidosis | **Serious** | **Expected** | Classified as **Serious** as lactic acidosis is a life-threatening metabolic condition and a medically important event. **Expected** as it is a known boxed-warning adverse reaction for Metformin. |
| **04** | Atorvastatin / Paracetamol (Statin/Analgesic) | Elevated liver enzymes | **Non-Serious** (or Medically Important if severe) | **Expected** | Asymptomatic mild-to-moderate transaminase elevation is generally **Non-Serious** and **Expected** in the product labeling, requiring routine monitoring or dose adjustment. |

---

## 3. Creating a Structured Case Classification Sheet (Tutorial Reference)

Based on the reference tutorial ([How to create a case classification sheet](http://www.youtube.com/watch?v=LHbUuZqadys)), structured case classification tables can also be built in qualitative/clinical data software to group cases by demographic and clinical attributes:

1. **Purpose of Case Classification:** Assigns demographic and clinical attributes (such as Gender, Age Group, Role, and Location) to individual study participants or patient cases so subgroups can be compared systematically.
2. **Creating the Classification Sheet:**
   * Navigate to the **Cases** directory and select **Case Classifications**.
   * Create a new classification sheet (e.g., `Participant Demographics Sheet` or `ADR Case Sheet`).
3. **Adding Attributes and Values:**
   * Right-click the classification table and add **New Attributes** (e.g., `Gender`, `Age Group`, `Seriousness`, `Expectedness`).
   * Open the **Values** tab (which includes default `Unassigned` and `Not Applicable` entries) and add specific values (such as `Male`/`Female`, `Serious`/`Non-Serious`, and `Expected`/`Unexpected`).
4. **Organizing Attributes:** Existing attributes from separate tables can be cut and pasted into a single master classification sheet to keep all case metadata consolidated before linking participant data.
5. 
