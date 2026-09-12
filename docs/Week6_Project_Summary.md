# Week 6 Project Summary - Data Analytics Track

## AnalystLab Africa Experience Lab | HealthConnect Clinic Project

## 1. What I Planned to Accomplish

Building on Week 5's initial EDA, KPIs, and insights, my goal for Week 6 was to deepen and validate the strongest findings, check whether any Week 5 conclusions needed revision, and produce a concrete cross-track deliverable for the Data Science track.

## 2. What I Completed

- Investigated whether booking lead time and prior no-show history compound when combined, rather than treating them as separate factors.
- Validated the reliability of the lead-time finding by checking it held consistently across all four appointment types.
- Validated the reminder-channel finding by checking it held consistently across lead-time bands.
- Produced an evidence-based Feature Relevance Summary ranking 8 candidate variables for predictive value.
- Exported this summary as a standalone file for the Data Science track.
- Refined business recommendations based on the deeper analysis.
- Updated the limitations section to reflect what was resolved, revised, and newly discovered.

## 3. What I Improved from Week 5

- Moved from single-factor analysis to combined risk-factor analysis (lead time × prior no-show history).
- Validated that key findings were not artifacts of one segment, but held consistently across appointment types.
- Revised an overly broad Week 5 conclusion (SMS as universally best) into a more accurate, lead-time-dependent recommendation.

## 4. What I Integrated

Produced a validated Feature Relevance Summary intended for direct use by the Data Science track in their Week 6 feature refinement process, based on the deeper validation analysis conducted this week.

## 5. Track(s) Collaborated With

Data Science (a real exchange with a Data Science intern working on the HealthConnect no-show prediction model).

## 6. What Was Exchanged

**Received:** Her actual Week 5 baseline model results - a Logistic Regression model achieving 63% accuracy, 62% recall, and 0.68 ROC-AUC, built using booking_lead_days, previous_no_shows, prior_no_show_rate, distance_to_clinic_km, appointment_type, reminder_sent, and reminder_channel. She specifically asked what strongest pattern from my analysis she hadn't tested yet.

**Provided:** Two specific, evidence-backed interaction-feature recommendations not currently in her model: (1) a lead-time × prior-no-show interaction (no-show rate compounds from 21.8% to 67.9% depending on the combination), and (2) a reminder-channel × lead-time interaction (her model treats reminder_channel independently, but its effectiveness changes depending on booking lead time - SMS is not universally best).

## 7. What Changed as a Result

Reviewing her actual notebook confirmed that my independent, descriptive-analysis approach and her formal statistical testing (t-tests and chi-square tests) reached full agreement on every candidate feature's relevance - a genuine cross-validation of both analyses. Beyond that agreement, she now has two specific, testable feature-engineering ideas to try against her existing 62% recall baseline, which she had not identified through her own testing.

## 8. Key Findings or Development Outcomes

- Lead time and prior no-show history compound: no-show rate ranges from 21.8% (lowest risk) to 67.9% (highest risk) depending on the combination.
- The lead-time effect is consistent across all appointment types, confirming it as a reliable, general pattern.
- The reminder-channel effect is not uniform - Email outperforms SMS for short-notice appointments, contradicting the Week 5 blanket recommendation.

## 9. Major Challenges

Deciding how to represent "cross-track integration" honestly, given I am working as an individual intern rather than paired with a live Data Science collaborator. Resolved by treating the shared, documented Data Science track requirements as the integration input, and producing a genuinely usable artifact as the output.

## 10. Important Decisions Made

- Chose to focus deeper analysis on only the two strongest Week 5 predictors (lead time, prior no-show history) rather than re-examining all six relationships, to keep the analysis focused and avoid repeating Week 5.
- Decided to explicitly revise the Week 5 reminder-channel conclusion rather than leave the outdated blanket recommendation standing, since the brief asks to review whether Week 5 conclusions need revision.

## 11. Remaining Issues

- All findings remain correlational, not causal - no controlled testing has been done.
- Dataset still lacks socioeconomic, insurance, and clinical-severity data.
- The revised reminder-channel finding should also be shared with the Generative AI track, since any assistant guidance mentioning reminder channels would currently be inaccurate.

## 12. Contribution to the Overall HealthConnect Project

Provided the Data Science track with a validated, evidence-backed feature prioritization that is more reliable than a general candidate list, directly supporting more efficient and accurate model development in their Week 6 work.

## 13. Proposed Focus for Week 7

- Support testing of the Data Science track's model using the validated features identified here, if their results are available for review.
- Explore whether a simple combined risk score (lead time + prior no-show) could be formalized into a specific scoring formula the clinic could use operationally.
- Communicate the revised reminder-channel finding to the Generative AI track if relevant to their assistant's content.