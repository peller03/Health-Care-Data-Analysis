# Healthcare-Analytics-Dashboard
---
## Table of Contents
- [Project Scope](#project-scope)
- [Data Sources](#data-sources)
- [Tool Used](#tool-used)
- [Data Cleaning & Preparation](#data-cleaning--preparation)
- [Exploratory Data Analysis Performed](#exploratory-data-analysis-performed)
- [EDA Visual Insights](#eda-visual-insights)
- [Data Analysis](#data-analysis)
- [Results / Findings](#results--findings)
- [Recommendations](#recommendations)

### Project Scope
This project analyzes clinical activity, patient encounters, diagnoses, and financial performance using Power BI.  
The objective is to uncover operational patterns, revenue gaps, and payer-related inefficiencies within a healthcare dataset.

The dashboard is designed to support:
- Executive-level performance monitoring
- Diagnosis and encounter-based clinical insights
- Financial and revenue cycle analysis using interactive root-cause exploration


![Health-Project_page-0001](https://github.com/user-attachments/assets/65982367-f67b-4e97-9388-6f0f627c8176)
 
---

### Data Sources
The dataset was sourced from a publicly shared healthcare dataset (X/Twitter Data analytics Challenge), consisting of **15 interrelated tables** covering clinical, operational, and financial records.

Supporting files include:
- patients.csv
- encounters.csv
- diagnoses.csv
- payers.csv
- providers.csv
- financials.csv
- calendar.csv
- data_dictionary.csv

---

### Tool Used
- Microsoft Power BI – Data modeling, DAX calculations, and dashboard development  
- Power Query – Data transformation, validation, and data type corrections  
- DAX – KPI creation, time intelligence, and financial performance calculations  

---

### Data Cleaning & Preparation
1. Validated and corrected data types across all tables (dates, currency, numeric fields).
2. Built a dedicated Calendar table to support time intelligence analysis.
3. Resolved many-to-many relationships using appropriate bridge tables.
4. Ensured financial metrics aligned correctly at the encounter-level grain.
5. Created calculated measures for charges, payments, allowed amounts, and revenue leakage.
6. Standardized categorical fields (encounter type, payer type, diagnosis descriptions).

---

### Exploratory Data Analysis Performed
The EDA focused on both clinical utilization and financial outcomes. Key KPIs explored include:
- Total Patients
- Total Encounters
- Total Diagnoses
- Total Charges
- Total Payments
- Revenue Leakage
- Collection Rate
- Readmission Rate
- Average Length of Stay

---

### EDA Visual Insights
- Encounter volume significantly exceeds patient count, indicating multiple visits per patient.
- A small subset of diagnoses accounts for a high proportion of total encounters.
- Inpatient encounters contribute disproportionately to overall revenue and payment gaps.
- Payment amounts consistently trail allowed amounts across payer categories.
- Monthly trends reveal variations in clinical activity and revenue generation.

---

### Data Analysis
Using DAX:
- SUM and DISTINCTCOUNT were used for volume-based metrics.
- Ratio measures were created for collection rate and diagnosis-per-encounter analysis.
- Time intelligence functions were applied to track year-over-year performance.
- A Decomposition Tree was implemented to perform root-cause analysis on payment gaps by encounter type, payer type, and year.

---

### Results / Findings
From the dashboard analysis:
- Inpatient encounters are the primary driver of the overall payment gap.
- Commercial and public payers contribute the largest share of revenue leakage.
- Financial performance varies more by payer and encounter type than by diagnosis volume alone.
- Year-over-year trends indicate gradual improvement in payment recovery.

---

### Recommendations
Based on the insights:
1. Focus revenue cycle improvement efforts on inpatient services.
2. Review reimbursement agreements with high-impact payer categories.
3. Monitor high-frequency diagnoses for operational efficiency.
4. Use root-cause analysis visuals to support targeted financial interventions.
5. Track payment gap trends over time to assess improvement initiatives.


 
