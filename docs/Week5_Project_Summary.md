# Week 5 Project Summary - Data Analytics Track

## AnalystLab Africa Experience Lab | HealthConnect Clinic Project

## 1. What I Planned to Accomplish

Building on the business questions and candidate KPIs identified in Week 4, my goal for Week 5 was to move from planning into actual analysis: preparing the data, exploring key relationships, calculating real KPI values, visualizing findings, and producing concrete business insights for HealthConnect.

## 2. What I Actually Completed

- Reviewed and confirmed data quality (data types, missing values, duplicates), and converted the date columns to proper date format.
- Filled missing `reminder_channel` values with "No Reminder" to support cleaner analysis.
- Explored relationships between appointment outcome and six factors: reminder channel, booking lead time, prior no-show history, distance to clinic, waiting time, and appointment type.
- Calculated 5 KPIs, each linked to a specific business question, with full interpretation.
- Built 5 visualizations covering the outcome distribution and the four strongest predictive relationships.
- Produced 5 business insights with clinic-relevant recommendations.
- Documented limitations and one cross-track collaboration point with the Data Science track.

## 3. Key Findings

- Nearly half (48.5%) of all appointments end in a no-show.
- Booking lead time is the strongest predictor: no-show rate rises from 27.8% (0-7 days) to 60.5% (31-60 days).
- Patients with a prior no-show have a 55.4% no-show rate vs. 43.5% for those with none.
- SMS reminders show the lowest associated no-show rate (45.8%) compared to no reminder (51.4%).
- Distance to the clinic has a moderate effect (46.5% within 5km vs. 54.1% at 15+km).
- Previous waiting time and appointment type showed little predictive value.

## 4. Major Challenges Encountered

The main challenge was deciding how to handle missing `reminder_channel` values in a way that kept analysis cleaner without deleting or distorting data. This was resolved by explicitly labeling them "No Reminder" rather than leaving them blank or dropping the rows.

## 5. Important Decisions Made and Why

- Converted `booking_date` and `appointment_date` from text to proper date format early on, since accurate date handling was needed for the lead-time analysis.
- Grouped continuous variables (booking lead days, distance, waiting time) into bands (e.g., 0-7 / 8-30 / 31-60 days) rather than analyzing raw values, to make patterns easier to interpret and communicate.
- Chose to build visualizations directly in the notebook rather than in Power BI, since it kept the analysis, code, and interpretation together in one place appropriate for this stage of the project.

## 6. Changes to My Week 4 Approach

No major changes - Week 5 followed the approach proposed in Week 4 closely. The main addition was deciding to band continuous variables (lead time, distance, waiting time) for clearer analysis, which wasn't explicitly planned in Week 4 but proved necessary once I started the actual calculations.

## 7. Cross-Track Collaboration Completed

Identified that the strongest KPI findings here (`previous_no_shows` and `booking_lead_days` as strong predictors) are directly relevant to the Data Science track's model feature selection, and that `waiting_time_minutes` showed weak predictive value and may be deprioritized in their feature set.

## 8. Remaining Work

- Deeper segmentation (e.g., combining distance and lead time) could be explored in a later stage.
- A formal statistical test (e.g., chi-square) could be added to confirm which relationships are statistically significant, not just descriptively different.

## 9. Proposed Focus for Week 6

- Explore combined/interaction effects between the strongest predictors (e.g., patients who both booked far in advance and have a prior no-show).
- Support the Data Science track's model development where useful, using the KPI findings identified here.
- Refine visualizations into a more polished, presentation-ready format if required for the final project deliverable
