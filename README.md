# Data-Cleaning-Power-Query
Excel, Power Query Project
![image](https://github.com/user-attachments/assets/301a0352-a51f-400a-8aaa-5f626841a310)

# Week 1 Data Challenge — Data Cleaning & Transformation

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## Project Overview

Welcome to my Week 1 Data Challenge repository! In this project, I embarked on an exciting data cleaning journey with a dataset from the challenge. The primary goal was to standardize, sanitize and structure the data to ensure it’s analysis-ready, reliable, and professional.

This process wasn’t just about code — it was about uncovering the story behind every value and preparing the dataset to deliver trustworthy insights that truly matter.

> *Special thanks and shoutout to [@Ifunanya Gabriel](https://github.com/IfunanyaGabriel) for the challenge!*

**Hashtags:**  
#datachallengewithIfunanyaGabriel  
#DCWeek1

---

## Table of Contents

- [Project Overview](#project-overview)  
- [Data Cleaning, Transformation & Insights](#data-cleaning-transformation--insights)  
- [Project Structure](#project-structure)  
- [before and after cleaning](#before-and-after-cleaning)  
- [Insights Generated](#insights-generated)  
- [Conclusion](#conclusion)

---

## Data Cleaning, Transformation & Insights

### Detailed Cleaning and Transformation

The dataset underwent a thorough cleaning and transformation process to ensure consistency, accuracy, and readiness for analysis. Key steps included:

1. **Data Import & Inspection**  
   Loaded the Excel workbook, selected the relevant worksheet (`Data Cleaning Task`), and conducted an initial review to identify data quality issues.

2. **Header Promotion and Standardization**  
   Promoted the first row as column headers, corrected column names for clarity, and ensured consistent naming conventions.

3. **Data Type Standardization**  
   Converted columns to appropriate data types:  
   - Names, emails, departments as strings  
   - Join Dates as datetime objects  
   - Age and Salary as numeric types

4. **Name Cleaning and Formatting**  
   - Capitalized each word in the Full Name column  
   - Removed non-printable characters and extra spaces  
   - Removed unnecessary punctuation  
   - Added spacing between concatenated names by detecting uppercase transitions. 
     *e.g., converted “MohamedAli” to “Mohamed Ali”*  
   - Manually fixed anomalies (e.g., changing “Anna- Marie O' Neil” to “Anna-Marie O'Neil”) for accuracy and respect to naming conventions

5. **Age Standardization**  
   - Converted written ages like “thirty” to numeric form (30)  
   - Replaced invalid or missing ages with nulls

6. **Email Address Cleanup**  
   - Lowercased all emails  
   - Removed duplicate `@` signs and ensured all emails ended with `.com`  
   - Flagged malformed emails for review

7. **Join Date Parsing**  
   - Converted text-based dates to valid date formats  
   - Replaced invalid dates with nulls for transparency

8. **Department Name Standardization**  
   - Capitalized department names uniformly  
   - Standardized common abbreviations (e.g., “Hr” to “HR”, “It” to “IT”)

9. **Salary Cleaning and Conversion**  
   - Removed commas and special characters  
   - Translated shorthand like “75k” to full numeric values (e.g., 75000)  
   - Converted salaries to numeric types and handled errors gracefully by replacing invalid entries with nulls

10. **Years of Service Calculation**  
    - Computed employee tenure as the difference between the current year and the join date year

11. **Missing Values Handling**  
    - Carefully assessed missing data per column based on its criticality  
    - Retained or imputed values as appropriate  
    - Avoided blind deletion to preserve data integrity and story

## Before and After Cleaning

<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/dbc49520-0c85-479c-895e-04aaa3675168" alt="Messy Data" width="400"></td>
    <td><img src="https://github.com/user-attachments/assets/5d761940-1e82-439f-8bcd-ea2a4432e72b" alt="Cleaned Data" width="400"></td>
  </tr>
  <tr>
    <td align="center"><b>Messy Data</b></td>
    <td align="center"><b>Cleaned Data</b></td>
  </tr>
</table>

---

### Insights Generated

After cleaning and preparing the dataset, several key insights emerged:

- **Average Age of Employees:** 39.7 years  
  This indicates a relatively mature workforce, which could influence benefits and development programs.

- **Total Salary Expense:** ₦685,030,000  
  Knowing the total salary outlay helps in budgeting, financial forecasting, and identifying cost-saving opportunities.

- **Years of Service Distribution:**  
  Calculating tenure highlighted employee retention trends and potential areas for HR focus.

- **Data Quality Reflection:**  
  The cleaning process uncovered common data entry errors and inconsistencies, underscoring the importance of data governance.

## Conclusion

This project went beyond technical cleaning — it was about respecting the data’s story, maintaining its meaning, and preparing it for actionable insights. By standardizing and validating each field thoughtfully, the dataset is now a trustworthy source for further analysis and decision-making.
