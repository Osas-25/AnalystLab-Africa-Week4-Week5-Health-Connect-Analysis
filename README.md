# HealthConnect Clinic - Data Analytics Track

## AnalystLab Africa Experience Lab Internship Programme

This repository contains my Week 4 and Week 5 submissions for the HealthConnect Clinic Experience Lab, part of the AnalystLab Africa internship programme.

## Project Background

HealthConnect Clinic is a fictional healthcare provider facing a high rate of missed patient appointments. The central project question is:

> **How can HealthConnect Clinic use data and AI to reduce missed appointments and improve the patient support experience?**

As part of the Data Analytics track, my role is to explore the appointment dataset, calculate meaningful KPIs, and produce insights that could help the clinic reduce no-shows and improve patient support.

---
## Repository Structure
```text
├── data/
│ └── HealthConnect_Appointment_Data.csv # Appointment dataset (5,000 records)
├── notebooks/
│ ├── Week4_Initial_Analysis.ipynb # Week 4: data quality review & initial analysis
│ └── Week5_Analytics_Report.ipynb # Week 5: EDA, KPIs, visualizations, insights
├── docs/
│ ├── Week4_Project_Summary.md
│ ├── Week5_Project_Summary.md
│ ├── chart1_outcome_distribution.png
│ ├── chart2_leadtime_noshow.png
│ ├── chart3_reminder_noshow.png
│ ├── chart4_history_noshow.png
│ └── chart5_distance_noshow.png
└── README.md
```

---
## Week 4 Progress

- Reviewed the dataset structure and confirmed data quality (no duplicates, no logical inconsistencies).
- Identified and explained missing values across three columns.
- Calculated the overall appointment outcome distribution (no-shows make up ~48.5% of appointments).
- Defined 5 business questions relevant to reducing no-shows.
- Identified 5 candidate KPIs, each linked to a business question.
- Outlined an initial analysis approach for Week 5.
- Documented assumptions, limitations, and risks affecting the analysis.

## Week 5 Progress

- Prepared the data further (fixed date formats, handled missing reminder values).
- Explored relationships between appointment outcome and 6 key factors: reminders, booking lead time, prior no-show history, distance to clinic, waiting time, and appointment type.
- Calculated 5 KPIs, each linked to a business question, with full interpretation.
- Built 5 visualizations to support the findings.
- Produced 5 business insights with recommendations for HealthConnect.
- Documented limitations and a cross-track collaboration point with the Data Science track.

## Key Findings (Week 5)

- ~48.5% of all appointments end in a no-show.
- Booking lead time is the strongest predictor: no-show rate rises from 27.8% (0-7 days) to 60.5% (31-60 days).
- Prior no-show history strongly predicts future no-shows (55.4% vs. 43.5%).
- SMS reminders are associated with the lowest no-show rate (45.8%) among all channels.
- Distance to clinic has a moderate effect (46.5% within 5km vs. 54.1% at 15+km).

## Tools Used

- Python (pandas, matplotlib)
- Jupyter Notebook

## Next Steps (Week 6)

- Explore combined/interaction effects between the strongest predictors.
- Support the Data Science track's modeling work using these KPI findings.
- Refine visualizations for a more polished, presentation-ready format.

---
*Part of the AnalystLab Africa Experience Lab Internship Programme.*

---
## Author 
**Angela Iseriehen**