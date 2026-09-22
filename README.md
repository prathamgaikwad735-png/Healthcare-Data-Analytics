# Healthcare Data Analytics

- An end-to-end Healthcare Data Analytics project focused on understanding patient demographics, medical conditions, treatment billing, insurance coverage, emergency admissions, and high-priority cases.

The project includes a Jupyter Notebook analysis and a self-contained interactive Executive Dashboard built from the analysis results.

## Dataset Used 
- <a href="https://github.com/prathamgaikwad735-png/Healthcare-Data-Analytics/blob/main/healthcare_dataset.csv">Dataset<a/>


# Open Interactive Dashboard

View Healthcare Executive Dashboard → https://prathamgaikwad735-png.github.io/Healthcare-Data-Analytics/healthcare_executive_dashboard.html

## Project Overview

- This project analyzes healthcare patient records covering May 2019 to May 2024. The analysis focuses on patient volume, medical conditions, age distribution, treatment billing, insurance coverage, emergency admissions, and cases that may require management review.

- Key Project Metrics

- KPI

- Value

- Patient Records After Cleaning

 54,966

- Average Billing Amount

  25,594.54

- Average Patient Age

51.5 years

- High-Cost Cases (> 90th Percentile)

5,497

- Emergency + Abnormal Test Result Cases

6,038

# Key Business Questions (KPIs)

## 1. Which medical condition affects the most patients?

- Finding:

Arthritis: 9,218 patients

Diabetes: 9,216

Hypertension: 9,151

Obesity: 9,146

Cancer: 9,140

Asthma: 9,095

<img width="866" height="378" alt="image" src="https://github.com/user-attachments/assets/293f657d-ad8b-433c-9dee-aec8b477a7f5" />


Management Insight: Arthritis has the highest patient count in the analyzed dataset, while Asthma has the lowest among the six listed conditions.

## 2. How is patient age distributed across the network?

- Finding:
The average patient age is approximately 51.5 years.

<img width="869" height="376" alt="image" src="https://github.com/user-attachments/assets/bafe5896-0d83-4418-ab06-498daf61d569" />


Management Insight: The patient population covers a broad age range, making age distribution useful for understanding healthcare demand across different patient groups.

## 3. How has average treatment cost changed over time?

- Finding:
Monthly average billing was analyzed across the May 2019–May 2024 reporting period.

<img width="892" height="395" alt="image" src="https://github.com/user-attachments/assets/118eeb5f-5ff2-45a4-9846-05310b46eea7" />


Management Insight: Monthly treatment-cost trends can help management monitor changes in average billing levels over time and identify periods that require further review.

## 4. Is there a relationship between patient age and treatment cost?

Finding:

- Overall average billing: 25,594.54

- Average billing for patients above 60 years: 25,529.85

  <img width="892" height="379" alt="image" src="https://github.com/user-attachments/assets/4113d117-9590-463e-ae85-03360c217029" />


Management Insight: The average billing for patients above 60 is slightly below the overall average in this dataset. The age-versus-billing relationship was also examined through a patient-level scatter analysis.

## 5. Which insurance provider covers the most patients?

Finding:

Cigna: 11,139

Medicare: 11,039

UnitedHealthcare: 11,014

Blue Cross: 10,952

Aetna: 10,822

<img width="884" height="450" alt="image" src="https://github.com/user-attachments/assets/e6bb5f8b-59c1-4d29-9912-dc1a9028472b" />


Management Insight: Cigna has the highest patient count among the insurance providers in the analyzed dataset.

## Process & Methodology

The project was completed through the following analytical process:

Data Loading

Loaded the healthcare dataset into a Pandas DataFrame.

Data Inspection

Reviewed dataset shape, columns, data types, missing values, duplicate records, and statistical summary.

Data Cleaning

Removed duplicate records.

Standardized patient names by removing extra spaces and applying title case.

Identified negative billing amounts and replaced them with the dataset mean billing value.

Converted admission and discharge dates into datetime format.

Created a length_to_stay field from admission and discharge dates.

Performed a final missing-value check.

Exploratory Analysis

Analyzed patient counts by medical condition.

Examined patient age distribution.

Analyzed monthly average billing.

Compared age with treatment cost.

Analyzed patient share by insurance provider.

Analyzed emergency admissions by month.

Management-Focused Analysis

Identified high-cost cases above the 90th percentile of billing.

Identified emergency patients with abnormal test results for priority review.

Tools Used

Python

Pandas

NumPy

Matplotlib

Jupyter Notebook

HTML / CSS / JavaScript for the interactive executive dashboard

## Dashboard Overview

The project includes an interactive Healthcare Executive Dashboard designed to present the analysis in a management-friendly format.

Dashboard Includes

Executive KPI cards

Patient and billing metrics

Medical condition analysis

Insurance provider analysis

Patient age insights

Emergency admission trends

High-cost case monitoring

Emergency patients with abnormal test results

Interactive filters

Interactive charts and hover details

Reset filters option

Responsive healthcare BI-style layout

Dashboard Filters

The dashboard supports relevant filters based on the available dataset, including:

Medical Condition

Insurance Provider

Gender

Admission Date / Year

# Dashboard Images

<img width="1355" height="636" alt="image" src="https://github.com/user-attachments/assets/51fa14a3-5b70-4edf-b4a1-c4a9ac0103ef" />

<img width="1332" height="451" alt="image" src="https://github.com/user-attachments/assets/a6b1364c-1aa5-4f53-80fd-a24d9cd56124" />

<img width="1331" height="417" alt="image" src="https://github.com/user-attachments/assets/576ee2bf-a9cf-42d5-a0f4-0beb17343d9b" />

<img width="1314" height="369" alt="image" src="https://github.com/user-attachments/assets/d72624a3-3666-47d9-88c9-57728d845dac" />

<img width="1338" height="595" alt="image" src="https://github.com/user-attachments/assets/e969d593-6d5b-4d68-819e-cd29d7def2fd" />

# Insights

Patient & Condition Insights

The dataset contains 54,966 cleaned patient records.

Arthritis has the highest patient count at 9,218.

The average patient age is approximately 51.5 years.

- Billing Insights

Average billing amount is 25,594.54.

Patients above 60 years have an average billing amount of 25,529.85.

5,497 cases fall above the 90th percentile of billing and were identified as high-cost cases for review.

- Insurance Insights

Cigna covers the highest number of patients with 11,139 records.

The five insurance providers have relatively close patient counts in the analyzed dataset.

Emergency Care Insights

A total of 18,502 emergency admissions were identified across the monthly emergency-admission analysis.

July recorded the highest number of emergency admissions: 1,573.

February recorded the lowest: 1,452.

6,038 emergency patients had abnormal test results and were identified as priority cases for review.

## Management Takeaways

Monitor the distribution of patients across medical conditions to understand healthcare demand.

Track monthly billing trends to identify periods with changes in average treatment cost.

Review high-cost cases separately to understand unusually high billing activity.

Monitor emergency admission patterns for capacity planning.

Prioritize emergency cases with abnormal test results for appropriate review.

Track insurance-provider patient distribution to understand the overall coverage mix.

🏁 Conclusion

This Healthcare Data Analytics project converts patient-level healthcare data into actionable management insights.

The analysis highlights patient volume, medical conditions, age distribution, treatment billing, insurance coverage, emergency admission patterns, high-cost cases, and priority emergency cases.

The accompanying interactive dashboard provides a concise executive view of these findings and makes the project suitable for demonstrating practical Data Analytics, Python, and Business Intelligence skills.

 Project Structure

Healthcare-Data-Analytics/
│
├── Health Care Analysis.ipynb
├── healthcare_executive_dashboard.html
└── README.md

👤 Project Focus

Healthcare Data Analytics | Exploratory Data Analysis | Business Insights | Executive Dashboard


