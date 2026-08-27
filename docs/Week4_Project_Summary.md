# Week 4 Project Summary - Data Analytics Track

## AnalystLab Africa Experience Lab | HealthConnect Clinic Project

## 1. The Problem My Track Will Address

My role as part of the Data Analytics track is to understand the HealthConnect appointment data well enough to figure out how it can help explain why patients miss their scheduled appointments. Specifically, I'm looking at which factors, like reminders, distance to the clinic, or a patient's past attendance history, are linked to no-shows, and how the clinic could measure and track this problem going forward.

## 2. Resources I Used

- **HealthConnect_Appointment_Data.csv** - the main dataset, containing 5,000 fictional appointment records for 1,696 unique patients.
- **HealthConnect Data Dictionary** - used to understand what each column in the dataset means.
- **Python (pandas) in Jupyter Notebook** - used to explore the data, check its quality, and calculate early observations.

## 3. Key Observations from Week 4

- The dataset is clean: there are no duplicate records and no logical errors (for example, no appointment was booked after it already happened).
- Some columns have missing values, but most of this is explainable rather than a mistake - for example, `reminder_channel` is only missing when no reminder was sent at all.
- Almost half of all appointments (about 48.5%) end in a no-show, which confirms this is a serious, ongoing problem for the clinic rather than a rare occurrence.
- Early comparisons suggest that patients who received a reminder had a slightly lower no-show rate, and patients who missed appointments before are more likely to miss future ones too.

## 4. My Proposed Approach

I identified five business questions and matched each one to a KPI (a measurement) that can answer it using the existing data - for example, tracking the overall no-show rate, how it changes by reminder status, and how it relates to a patient's past no-show history. In Week 5, I plan to calculate these KPIs properly, break them down by patient group, and start putting together simple charts or a dashboard to show the results clearly.

## 5. Key Considerations That May Affect the Project

- The dataset doesn't include some information that might affect no-shows in real life, like a patient's income or how serious their medical condition is.
- The patterns I've noticed so far (like reminders being linked to fewer no-shows) are just early observations - they don't prove that one thing directly causes the other.
- I'll need to stay in touch with the Data Science and Generative AI tracks to make sure we're all treating things like "no-show" and "cancelled" the same way, so our final project pieces fit together properly.

## 6. Proposed Focus for Week 5

- Calculate the five KPIs identified in Week 4.
- Break the results down by patient age group, appointment type, and time of day.
- Look more closely at how reminders, booking lead time, and past no-show history relate to attendance.
- Start planning a simple dashboard to present the findings clearly.