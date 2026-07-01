# Hospital-Emergency-Room-Analysis
To enhance overall efficiency and provide actionable insights into Emergency room performance, we need to create a Hospital Emergency Room Analysis Dashboard in Power Bi. This solution will enable stakeholders to track, analyze, and make data driven decisions regarding patient management and service optimization.

## Dashboard Preview
## 1. Monthly View Dashboard
Objective: Monitor key metrics and trends on a month-by-month basis to identify patterns and areas for improvement.

Layout:
- Patient Admission Status: Track admitted vs non admitted patients.
- Patient Age Distribution: Group patients by 10-year age interval.
- Department Referrals: Analyze referral trends across different departments.
- Timeliness: Measure the percentage of patients seen within 30 minutes.
- Gender Analysis: Visualize patient distribution by gender.
- Racial Demographics: Analyze patient data by race.
- Time Analysis: Assess patient volume by day and hour.

Key Metrics:
-	Number of Patients
-	Average Wait Time
-	Patient Satisfaction Score
-	Number of Patients Referred
  
<img width="910" height="505" alt="Monthly View Dashboard Screenshot" src="https://github.com/user-attachments/assets/c15e8ac1-434a-4cf4-b96d-5a2786c72f7d" />


## 2. Consolidated View Dashboard
Objective: Provide a holistic summary of hospital performance from a selected date range.

Layout: Similar to monthly view dashboard, but aggregated over a customizable date range for broader insights and trend analysis.

<img width="916" height="507" alt="Consolidated view Dashboard Screenshot" src="https://github.com/user-attachments/assets/4ee54359-98b3-4eb1-a0f1-9e382c039907" />


## 3. Patient Details Dashboard
Objective: Offer granular insights into patient-level data to enable detailed analysis and troubleshooting.

Layout: A grid displaying essential fields:
- Patient ID
- Patient Full Name
- Gender
- Age
- Admission Date
- Patient Race
- Wait Time
- Department Referral
- Admission Status

<img width="917" height="497" alt="Patient Details Dashboard" src="https://github.com/user-attachments/assets/1fcd9a7a-9732-4016-bebc-2e94c82cc273" />

## 4. Key Takeaways

Objective: Summarize the findings from all dashboards to provide clear and actionable insights from stakeholders.

Layout:
Descriptive analysis of each metric and visualization, including patterns, anomalies, and actionable recommendations to optimize emergency room operations and patients care.

<img width="916" height="499" alt="KeyTakeaways Dashboard Screenshot" src="https://github.com/user-attachments/assets/25dd297b-ad6d-46c4-8531-447b5cd4860e" />

 ## Tools Used
- Power Bi
- Power Query
- DAX

## Data Preparation - Power Query
- Changed the first row to be headers
- Merged the patient first name initial and patient last name into patient name column
- Replaced F with Female and M with Male in the Patient Gender column
- Added a conditional column called patient admission flag 2  to group patient admission flag into: 1 = true and else = false and removed the original patient admission flag column

## DAX Measures
- Average wait time
- Number of patients
- Number of patients referred
- Patient satisfaction score
- Created Date Table
  
## Objectives
- To enhance overall efficiency and provide actionable insights into Emergency room performance.

## Analysis
-	Key performance indicators (KPI's): Number of Patients, Average Wait Time, Patient Satisfaction Score and Number of Patients Referred.
-	Patient Admission Status: Track admitted vs non admitted patients.
- Patient Age Distribution: Group patients by 10-year age interval.
- Department Referrals: Analyze referral trends across different departments.
- Timeliness: Measure the percentage of patients seen within 30 minutes.
- Gender Analysis: Visualize patient distribution by gender.
- Racial Demographics: Analyze patient data by race.
- Time Analysis: Assess patient volume by day and hour.

## Filters
- Month Year
- Date range
  
## Key Findings and Insights
- The Emergency Room Dataset covering a period of 19 months, records a total of 9,216 unique patients
- Patient Wait Time Satisfaction: 
The average wait time was approximately 35.3 minutes, indicating a need for improvement to enhance patient flow. The Average satisfaction was 5.0 out of 10 suggesting moderate satisfaction and highlighting areas for improving patient experiences.
- Department Referrals:
A significant number of patients (5400) did not require referrals. Among those referred the most common were General Practice (1840 cases)  and orthopedics (995 cases), followed by physiotherapy  (276 cases) and cardiology (248 cases)
- Peak Busy Periods:
The busiest days were Mondays (1377 patients), Saturdays (1322 patients) and Tuesdays (1318 patients). The busiest hours were 11 AM, 7 PM, 1 PM, and 11 PM indicating need of ample staffing during these periods.
- Patient Demographics:
Age Groups: Adults (30-39 years) formed a large group (1200 patients), followed by young adults (20 -29 years) with 1188 patients. Other significant groups included middle aged as well (40 - 50 years).
- Race Distribution:
The largest racial group was white (2571), followed by African American (1951), Multiracial (1557), and Asian (1060) patients. A significant number of patients (1030) declined ti identify their race.
- Admission Patterns
Nearly half of the patients (4612) were admitted while the rest (4604) were treated and released.
  
## Conclusion
The dataset reveals that high patient volumes, moderate satisfaction levels, and common referrals to general practice and orthopedics. Mondays and late nights to early morning hours are particularly busy. The patient demographics show a diverse age and racial composition with nearly equal numbers of admitted and non admitted patients. These insights can help optimize resource allocation and improve patient care in the emergency room.

 ## Recommendations
- Reduce Patient Wait Times:
Review and optimize patient triage and registration processes to reduce the average wait time of 35.3 minutes.
Introduce fast-track services for patients with minor conditions to improve patient flow and decrease congestion.

- Improve Patient Satisfaction:
Conduct patient feedback surveys to identify the main causes of the moderate satisfaction score (5.0/10).
Enhance communication by providing patients with regular updates on expected waiting times and treatment progress.

- Optimize Staffing During Peak Periods:
Increase staffing levels on Mondays, Tuesdays, and Saturdays, as well as during the busiest hours (11 AM, 1 PM, 7 PM, and 11 PM).
Use historical patient volume data to create demand-based staff schedules.

- Strengthen Coordination with High-Demand Departments
Improve collaboration with General Practice and Orthopedics, which receive the highest number of referrals.
Consider allocating additional specialists or establishing streamlined referral pathways to reduce delays.

- Plan Services Around Patient Demographics:
Ensure adequate resources and services are available for adults aged 20–39 years, who represent the largest patient population.
Develop targeted health education and preventive care initiatives for common conditions affecting these age groups.

- Enhance Capacity Planning:
Since admissions and discharges occur in nearly equal proportions, maintain adequate bed availability while ensuring efficient discharge planning to prevent overcrowding.
Regularly monitor occupancy rates to support effective resource allocation.

- Improve Data Collection Practices:
Encourage patients to voluntarily provide demographic information, including race, to support more comprehensive analyses of healthcare utilization and equity.
Periodically review data quality to ensure accurate reporting and informed decision-making.

- Implement Continuous Performance Monitoring:
Develop a dashboard to track key performance indicators (KPIs) such as patient wait time, satisfaction scores, referral trends, admission rates, and patient volumes.
Regular monitoring will enable hospital management to identify trends early and implement timely operational improvements.
