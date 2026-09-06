# ASG Airlines: End-to-End Data Engineering & Operational Analytics Case Study


**Role:** Data Engineer  
**Tools Used:** Python (Pandas, NumPy), Power BI Desktop, Draw.io  

---

## Project Overview
This project delivers an automated data engineering pipeline and an interactive Power BI dashboard for ASG Airlines. The pipeline ingests multi-sheet operational data (flights, passengers, bookings, and payments), cleans data quality anomalies, protects sensitive passenger information, and models the clean data into a Star Schema for business intelligence reporting.

---

## Key Pipeline Highlights
* **Deduplication:** Removed 15 duplicate flight records, resulting in 1,005 clean flight operations.
* **Airline Imputation:** Standardized missing airline names using flight number prefixes (e.g., AI for Air India, 6E for IndiGo).
* **Overnight Flight Correction:** Handled 122 cross-midnight flights by applying a +24 hour formula, establishing the true network average flight duration of 2.74 hours.
* **Data Privacy (PII Masking):** Masked Aadhaar numbers, phone numbers, passport details, and emails in the storage layer, and excluded all PII from the Power BI reporting dataset (Data Minimization).
* **Anomaly Handling:** Standardized 75 corrupted booking statuses into an UNKNOWN category and flagged 78 non-numeric payment amounts without data loss.
* **Data Modeling:** Built a Star Schema in Power BI centered on bookings with zero orphaned foreign keys.

---

