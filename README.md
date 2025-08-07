#  Hospital Management SQL Analytics Dashboard 

## 1.  Background and Overview

This project focuses on analyzing and optimizing patient flow, doctor utilization, and revenue streams in a multi-specialty hospital setting. Using SQL queries and Power BI visualization, the dashboard provides actionable insights across patient demographics, treatments, billing, and operational inefficiencies.

The goal is to assist hospital administrators and decision-makers in improving patient care delivery, resource allocation, and financial management.

---

## 2.  Data Structure and Overview

The analysis is based on a normalized healthcare database with 6 core entities:

###  `patients` 
 Column Description
-  patient_id -> Unique ID for each patient
- first_name -> Patient's first name
- last_name -> Patient's last name
- gender -> Gender (M/F)
- date_of_birth -> Date of birth
- contact_number -> Phone number
- address -> Address of the patient
- registration_date -> Date of first registration at the hospital
- insurance_provider -> Insurance company name
- insurance_number -> Policy number
- email -> Email address

###  `doctors`  
 Column Description
- doctor_id -> Unique ID for each doctor
- first_name -> Doctor's first name
- last_name -> Doctor's last name
- specialization -> Medical field of expertise
- phone_number -> Contact number
- years_experience -> Total years of experience
- hospital_branch -> Branch of hospital where doctor is based
- email -> Official email address

###  `appointments`
 Column Description
- appointment_id -> Unique appointment ID
- patient_id -> ID of the patient
- doctor_id -> ID of the attending doctor
- appointment_date -> Date of the appointment
- - appointment_time -> Time of the appointment
- reason_for_visit -> Purpose of visit (e.g., checkup)
- status -> Status (Scheduled, Completed, Cancelled)

###  `treatments` 
- Column Description
- treatment_id -> Unique ID for each treatment
- appointment_id -> Associated appointment ID
- treatment_type -> Type of treatment (e.g., MRI, X-ray)
- description -> Notes or procedure details
- cost -> Cost of treatment
   
###  `billing`
-  Column Description
- bill_id -> Unique billing ID
- patient_id -> ID of the billed patient
- treatment_id -> ID of the related treatment
- bill_date -> Date of billing
- amount -> Total amount billed
- payment_method -> Mode of payment (Cash, Card, Insurance)
- payment_status -> Status of payment (Paid, Pending, Failed)

 ---

## 3.  Executive Summary

The dashboard uncovered several operational pain points in the hospital’s current setup:

- Uneven patient load distribution among doctors on peak days
- Over-reliance on a few high-performing doctors and treatments
- 30+ day unpaid bills contributing to poor cash flow
- High-value patients concentrated under select insurance providers

This highlights the need for a better scheduling system, targeted treatment planning, and more balanced insurance partnerships.

---

## 4.  Insights Deep Dive

-  **Unpaid Bills > 30 Days**  
  → Indicates bottlenecks in collections; impacting liquidity.

-  **Doctor Revenue & Utilization**  
  → Small group of doctors generate over 50% of revenue. Others underutilized.

-  **Top 5 Treatments**  
  → Repeat elective procedures make up majority of revenue — opportunity to optimize or scale.

-  **Revenue Seasonality**  
  → Revenue dips in Q3; demand planning needed for that period.

-  **Gender-based Diagnosis Trends**  
  → Certain conditions skewed by gender — useful for resource prep.

-  **Insurance Provider Load**  
  → Top 2 insurance companies cover majority of patients — risky dependency.

---

## 5.  Recommendations

-  **Dynamic Doctor Scheduling**  
  Use historical demand data to allocate doctors more efficiently during peaks.

-  **Improve Collections on Overdue Bills**  
  Set alerts, offer discounts for early payments, or escalate chronic defaulters.

-  **Treatment Portfolio Optimization**  
  Focus on high-value treatments with lower cancellation rates.

-  **Diversify Insurance Partnerships**  
  Reduce revenue risk by onboarding additional insurance providers.

-  **Leverage Elective Procedure Demand**  
  Launch packages/promotions during off-peak seasons to stabilize revenue.

---

##  Tools Used

- **SQL** – Data extraction, Data cleaning and Analysis
 

##  By

**Girish K S**  
🔗 [girishhemanth823@gmail.com] 
 

---

