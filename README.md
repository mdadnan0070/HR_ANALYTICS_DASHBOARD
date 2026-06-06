# HR_ANALYTICS_DASHBOARD
HR Analytics Dashboard built with Python and Power BI on IBM HR dataset to analyze employee attrition, satisfaction and compensation.

# HR Analytics Dashboard

## Overview
An interactive HR Analytics Dashboard built using Python and Power BI on the IBM HR Employee Attrition dataset from Kaggle.

## Tools Used
- **Python (pandas)** — data cleaning and transformation
- **Power BI** — dashboard and DAX measures
- **Dataset** — IBM HR Analytics (synthetic, publicly available on Kaggle)

## Data Cleaning (Python)
- Dropped 6 useless columns: `EmployeeCount`, `Over18`, `StandardHours`, `HourlyRate`, `DailyRate`, `MonthlyRate`
- Mapped numeric codes to readable labels (Education, Job Satisfaction, Performance Rating etc.)
- Created Age Group and Tenure Group bins
- Added satisfaction score columns for gauge visuals

## Dashboard Pages

### Page 1 — Overview
- KPIs: Total Employees, Male/Female split, Attrition Count, Attrition Rate, Average Salary, Age, Tenure
- Charts: Attrition by Age Group, Attrition by Education Field
- Gauges: Performance Rating, Work Life Balance, Job Satisfaction, Job Involvement

### Page 2 — Attrition Analysis
- Attrition by Job Satisfaction
- Attrition by Job Role
- Attrition by Tenure Group
- Attrition by Department

## Key Insights
- Overall attrition rate: **16.12%**
- Sales Representatives have the highest attrition: **39.76%**
- Employees with **0-4 years tenure** are most at risk (24.31%)
- **Low job satisfaction** drives the most attrition (22.84%)
- **26-35 age group** has the highest attrition count (116 employees)
- **Life Sciences** education field has most attrition (89 employees)

## How to Run
1. Download dataset from Kaggle: IBM HR Analytics Employee Attrition
2. Run `hr_cleaning.py` to generate `hr_cleaned.csv`
3. Open `HR_Dashboard.pbix` in Power BI Desktop
4. Refresh data source pointing to `hr_cleaned.csv`
