Telco Customer Churn Analysis
Overview
This project focuses on analyzing customer churn for a telecommunications company. The main objective is to clean the raw customer dataset, calculate key performance indicators (KPIs), and explore the underlying factors contributing to customer attrition using Google Sheets.

Dataset Summary
The dataset contains customer demographic information, subscribed services, account details, and churn status:

Total Customers Analyzed: 7,043

Churned Customers: 1,869

Overall Churn Rate: 26.54%

Average Monthly Charge: ~$64.76

Methodology & Steps Completed
1. Data Cleaning & Import
Imported the raw dataset (cleaned_telco_churn.csv) into Google Sheets.

Ensured consistent formatting across all numerical and categorical columns.

2. KPI Metrics Calculation
Created a dedicated KPIs summary tab using dynamic Google Sheets formulas:

Total Customers: =COUNTA(cleaned_telco_churn!A2:A)

Churned Customers: =COUNTIF(cleaned_telco_churn!U2:U; "Yes")

Churn Rate: =B3/B2 (formatted as percentage)

Average Monthly Charges: =AVERAGE(cleaned_telco_churn!S2:S)

3. Exploratory Data Analysis (Pivot Tables & Charts)
Built interactive Pivot Tables and visualizations on the Analyse tab to identify key churn drivers:

Contract Type Analysis: Evaluated churn distribution across Month-to-month, One year, and Two year contracts using a stacked column chart (Churn Rate by Contract Type).

Payment Method Analysis: Analyzed customer retention across Electronic check, Mailed check, Bank transfer (automatic), and Credit card (automatic) using a secondary breakdown chart (Churn Rate by Payment Method).

Key Insights & Findings
Contract Length: Customers on Month-to-month contracts exhibit the highest churn rate. Long-term contracts (1 or 2 years) show significantly higher retention rates.

Payment Method: Customers using Electronic check as their payment method display a noticeably higher tendency to churn compared to those using automated payment methods (bank transfers or credit cards).
