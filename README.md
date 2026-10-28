# Fintech Cohort Analysis: Customer Retention & Engagement

## Project Overview

This project analyzes customer retention patterns in a fintech dataset using cohort analysis. Customers are grouped according to the month of their first recorded transaction, allowing retention performance to be compared across different customer acquisition cohorts.

The analysis uses Python, Pandas, Matplotlib, and Seaborn to calculate monthly retention rates and visualize customer activity over time.

## Business Objectives

- Understand customer retention patterns over time.
- Group customers by their first transaction month.
- Calculate monthly cohort retention rates.
- Identify cohorts with the highest and lowest Month 1 retention.
- Visualize retention trends using a cohort heatmap.
- Export the retention table for further analysis.

## Dataset

**Source file:** `Assignment Cohort Data - Fintech Data.xlsx`

The notebook references the following columns:

- `date` — transaction date.
- `username` — customer identifier.
- `revenue` — revenue associated with a transaction.

The dataset's full structure, date range, and data quality should be verified using the notebook's inspection outputs.

## Tools & Technologies

- Python
- Pandas
- Matplotlib
- Seaborn
- Google Colab
- Excel

## Methodology

### 1. Data Preparation

Load the Excel dataset, inspect its dimensions and data types, check missing values, and convert the transaction date to datetime format.

### 2. Cohort Assignment

Assign each customer to a cohort based on the month of their first recorded transaction.

### 3. Cohort Index Calculation

Calculate the number of months between each transaction month and the customer's cohort month.

### 4. Retention Rate Calculation

Calculate retention by dividing the number of distinct customers active in each cohort month by the number of distinct customers in that cohort's initial month.

### 5. Retention Visualization

Create a heatmap to compare retention percentages across cohorts and elapsed months.

### 6. Cohort Comparison

Compare Month 1 retention across cohorts and calculate average retention across the available periods for each cohort.

### 7. Export Results

Export the retention table to `cohort_retention.csv` for further analysis.

## Key Outputs

- Cohort membership table.
- Monthly cohort activity table.
- Customer retention rate table.
- Cohort retention heatmap.
- Month 1 retention ranking.
- Exportable CSV file.

## Business Value

Cohort analysis helps fintech businesses understand whether customers continue using their services after their first recorded transaction. The results can support further investigation into customer engagement, onboarding, and retention strategies.

Specific business recommendations should be based on the actual retention results and additional customer behavior data.

## Limitations

- Retention is measured using distinct customers with recorded transactions; it does not necessarily measure app logins or other forms of engagement.
- The dataset alone does not establish why customers stop transacting.
- Recent cohorts may have incomplete observation periods and should not be compared directly with older cohorts without accounting for this limitation.
- Revenue analysis is not yet included in the retention calculations.

## Author

**Risty Anugrah Dwi Septiana**

Informatics Engineering Graduate | Data Analyst Enthusiast

- GitHub: [Ristyanugrah](https://github.com/Ristyanugrah)
- Portfolio: [Data Analytics Portfolio](https://github.com/Ristyanugrah/data-analytics-portfolio)
