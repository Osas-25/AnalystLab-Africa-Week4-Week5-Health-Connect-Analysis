# HealthConnect Clinic — Data Analytics Track

## AnalystLab Africa Experience Lab Internship Programme

This repository contains my Week 4, Week 5, and Week 6 submissions for the HealthConnect Clinic Experience Lab, part of the AnalystLab Africa internship programme.

## Project Background

HealthConnect Clinic is a fictional healthcare provider facing a high rate of missed patient appointments. The central project question is:

> **How can HealthConnect Clinic use data and AI to reduce missed appointments and improve the patient support experience?**

As part of the Data Analytics track, my role is to explore the appointment dataset, calculate and validate meaningful KPIs, and produce insights and evidence-based recommendations that support HealthConnect's decision-making — including findings that feed directly into the Data Science track's modeling work.

## Repository Structure
```text
├── data/
│ └── HealthConnect_Appointment_Data.csv # Appointment dataset (5,000 records)
├── notebooks/
│ ├── Week4_Initial_Analysis.ipynb # Week 4: data quality review & initial analysis
│ ├── Week5_Analytics_Report.ipynb # Week 5: EDA, KPIs, visualizations, insights
│ └── Week6_Advanced_Analytics.ipynb # Week 6: validation, combined risk analysis, integration
├── docs/
│ ├── Week4_Project_Summary.md
│ ├── Week5_Project_Summary.md
│ ├── Week6_Project_Summary.md
│ ├── DataScience_Feature_Relevance_Summary.csv # Cross-track integration artifact for Data Science
│ ├── chart1_outcome_distribution.png
│ ├── chart2_leadtime_noshow.png
│ ├── chart3_reminder_noshow.png
│ ├── chart4_history_noshow.png
│ ├── chart5_distance_noshow.png
│ └── chart6_combined_risk.png
└── README.md
```

---

## Week 4 Progress
- Reviewed dataset structure and confirmed data quality.
- Identified 5 business questions and 5 candidate KPIs.

## Week 5 Progress
- Prepared the data further and explored 6+ key relationships.
- Calculated and interpreted 5 KPIs.
- Built 5 visualizations and produced 5 business insights.

## Week 6 Progress
## Week 6 Progress
- Investigated whether the two strongest Week 5 predictors (booking lead time, prior no-show history) compound when combined - confirmed they do (no-show rate ranges from 21.8% to 67.9% depending on the combination).
- Validated the lead-time finding for consistency across all appointment types.
- Validated and **revised** the Week 5 reminder-channel conclusion - SMS is not universally best; effectiveness depends on lead time.
- Collaborated directly with a Data Science intern: reviewed her actual Week 5 baseline model (Logistic Regression, 63% accuracy, 62% recall, 0.68 ROC-AUC) and provided two specific, evidence-backed interaction-feature recommendations not yet in her model.
- Cross-validated my feature relevance findings against her independent statistical testing (t-tests, chi-square) - found full agreement across every candidate feature.
- Produced a validated Feature Relevance Summary, updated to include this cross-validation, as a cross-track integration deliverable.
- Refined business recommendations based on the deeper analysis.

## Key Findings (Updated Through Week 6)

- ~48.5% of all appointments end in a no-show.
- Booking lead time and prior no-show history compound: no-show rate ranges from 21.8% (short lead time, no prior no-show) to 67.9% (long lead time, prior no-show).
- Reminder channel effectiveness depends on lead time - Email performs best for short-notice appointments, SMS for longer lead times.
- Distance to clinic has a moderate effect (46.5% within 5km vs. 54.1% at 15+km).

## Tools Used

- Python (pandas, matplotlib)
- Jupyter Notebook

## Cross-Track Integration

Week 6 involved a real exchange with a Data Science intern building the HealthConnect no-show prediction model. After reviewing her actual baseline results, I provided two specific interaction-feature recommendations (lead-time × prior-no-show, and reminder-channel × lead-time) that were not yet tested in her model. This is documented in `docs/DataScience_Feature_Relevance_Summary.csv` and in the Week 6 notebook.

## Next Steps (Week 7)

- Support testing of the Data Science track's model using the validated features identified here.
- Explore formalizing a combined risk score (lead time + prior no-show) for operational use.
- Communicate the revised reminder-channel finding to the Generative AI track if relevant to their assistant.

---
*Part of the AnalystLab Africa Experience Lab Internship Programme.*

---
## Author 
**Angela Iseriehen**