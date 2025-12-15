DEA on hospital data for Operations Research Management   project

# ⚕️ Hospital Efficiency Analysis: Data Envelopment Analysis (DEA) in R

##  Overview
 Our focus was on applying **Data Envelopment Analysis (DEA)** to evaluate the operational efficiency of hospitals in Oregon.

The core problem in healthcare is maximizing patient care quality while minimizing resource use. Our goal was simple: **Identify which Oregon hospitals are the most efficient at turning limited resources (inputs) into positive patient outcomes (outputs).**

The entire project—from data cleaning to the final efficiency scoring—was conducted in **R**.

## What's  Inside?

| File | Description |
| :--- | :--- |
| `hospital_efficiency.R` | The main R script containing all the DEA calculations and efficiency scoring. |
| `ETM540 Final Project Report.docx` | The complete, detailed academic report outlining the literature review, methodology, data sources, and final conclusions. |
| `ETM540 Final Presentation Team 3.pptx` | The comprehensive slide deck summarizing our methodology and results for the final presentation. |
| `Combined_Hospital_Data_OR.csv` | The clean, pre-processed dataset from the Centers for Medicare & Medicaid Services (CMS) used for the analysis, focusing on Oregon facilities. |

## Methodology: Data Envelopment Analysis (DEA)

We used **DEA**, a non-parametric method from Operations Research, to measure the relative efficiency of multiple Decision Making Units (DMUs)—in this case, hospitals. DEA is highly effective because it can handle multiple inputs and outputs simultaneously without requiring assumptions about their relationship.

* **Inputs (Resources Consumed/Inefficiency Indicators):** We focused on the **Predicted Readmission Rate**, which is a strong proxy for suboptimal resource utilization (as poor initial care leads to resource-consuming readmissions).
* **Outputs (Results Delivered/Quality):** We measured patient service and quality using the **Number of Discharges** (service volume) and the **Number of No Readmissions** (quality of care).
* **Hypothesis:** Facilities with lower predicted readmission rates and a high number of discharges will be more efficient.

### **Our Key Findings**

The DEA model successfully calculated efficiency scores (both Constant Returns to Scale - CRS and Variable Returns to Scale - VRS) for the Oregon hospitals. The analysis identified the relative efficiency frontier, pinpointing top-performing hospitals that serve as benchmarks for those with lower efficiency scores.

* **Top Scorers:** Hospitals on the efficiency frontier demonstrate the best practices in resource management and patient care delivery.
* **Low Scorers:** Hospitals with low scores offer clear opportunities for operational improvement by studying the input/output ratios of the benchmark facilities.

## Future Work & Improvements

While the study achieved its academic objective, future analysis could be enhanced by:

1.  **Expanded Data:** Utilizing a larger dataset or comparing efficiency across two states with similar populations.
2.  **Additional Metrics:** Incorporating inputs like total cost invested in the hospital, patient satisfaction scores, or staff-to-patient ratios for a more comprehensive view.
3.  **Departmental Analysis:** Applying DEA to individual departments within a single company or hospital to identify internal areas for optimization.
