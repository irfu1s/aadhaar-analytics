# Aadhaar Analytics  
### Enrollment vs Demographic Update Patterns at National Scale

## Overview

This project performs a large-scale analytical comparison of Aadhaar **initial enrollments** and **subsequent demographic updates** to understand how India’s identity system has evolved from a one-time registration mechanism into a continuous identity maintenance platform.

The work focuses on measuring **operational load**, identifying **regional disparities**, and extracting **policy-relevant insights** using a reproducible analytics workflow built primarily with **Python, Pandas, and Power BI**.

The emphasis of this project is on **descriptive and diagnostic analytics**, not predictive modeling.

---

## Problem Statement

Aadhaar was originally designed as a one-time enrollment system.  
Over time, demographic updates such as address changes, mobile number updates, and identity corrections have grown substantially.

This project addresses the following questions:

- How does the scale of demographic updates compare to new enrollments?
- Which regions contribute most to Aadhaar’s ongoing operational workload?
- What does this transition imply for long-term identity system planning and policy design?

---

## Data Sources

The analysis uses two official Aadhaar public datasets obtained via UIDAI APIs:

- Aadhaar Enrollment Dataset  
- Aadhaar Demographic Update Dataset  

Both datasets are national in scope and contain multi-year, state-level temporal data.

---

## Analytics Workflow

The project follows a clear, analytics-first workflow.

Raw data is collected and preserved without modification.  
Cleaned datasets are produced through validation and standardization steps.  
The cleaned datasets are then merged to enable comparative analysis.  
Insights are explored and validated using Jupyter notebooks.  
Final results are communicated through Power BI dashboards.

---

## Project Structure

The repository is organized to reflect the full lifecycle of an analytics project, from raw data ingestion to final reporting.

```
aadhaar-analytics/
│
├── Data/
│   ├── Raw/
│   │   ├── api_data_aadhaar_enrolment.zip
│   │   └── api_data_aadhaar_demographic.zip
│   │
│   ├── Processed/
│   │   ├── aadhaar_enrolment_cleaned.csv
│   │   └── aadhaar_demographic_cleaned.csv
│   │
│   └── Merged/
│       └── ml_df.csv
│
├── Notebooks/
│   ├── 01_data_ingestion.ipynb
│   └── 02_analysis_insights.ipynb
│
├── Power BI Dashboards/
│   ├── Comparison_Dashboard_.pbix
│   ├── Comparison_Dashboard_Image.jpg
│   │
│   ├── Demographic_Dashboard_.pbix
│   ├── Demographic_Dashboard_Image.jpg
│   │
│   ├── Enrolment_Dashboard_.pbix
│   └── Enrolment_Dashboard_Image.jpg
│
|
|- Project_report
|
└── README.md
```

---

## Folder Details

**Data/**  
Contains all datasets used in the analysis, organized by processing stage.

- **Raw/** holds the original API-downloaded datasets in compressed form.
- **Processed/** contains cleaned and standardized CSV files.
- **Merged/** contains the final merged dataset used for comparative analysis.

**Notebooks/**  
Contains Jupyter notebooks used for data ingestion, validation, exploration, and analytical insight generation.  
Notebook execution order is reflected in the numeric prefixes.

**Power BI Dashboards/**  
Contains interactive Power BI dashboards (`.pbix`) along with exported `.jpg` snapshots for quick preview and documentation.  
Each dashboard focuses on a distinct analytical perspective: Enrollment, Demographic Updates, and Comparative Analysis.

---

## Key Insights

- Demographic updates represent a **substantially higher operational workload** than new Aadhaar enrollments.
- Several states exhibit **high update-to-enrollment ratios**, indicating sustained identity maintenance pressure.
- Aadhaar has effectively transitioned into a **long-term identity lifecycle system**, not a one-time registration program.

---

## Impact & Use Cases

This analysis can support:

- Operational planning for UIDAI and enrollment agencies
- Evidence-based policy evaluation of Aadhaar lifecycle management
- Resource allocation decisions based on regional update intensity

---

## Tools & Technologies

- Python (Pandas, NumPy)
- Jupyter Notebooks
- Power BI
- CSV-based analytical datasets

---

## Notes

This project prioritizes **interpretability, auditability, and policy relevance** over model complexity.  
The objective is to support **decision-making and public policy analysis**, not machine learning performance benchmarks.

---

## Author

K Mohammad Irfan Hussain  
Data Science Undergraduate  
Focus: Analytics, Public Policy Systems, Financial Data Infrastructure
