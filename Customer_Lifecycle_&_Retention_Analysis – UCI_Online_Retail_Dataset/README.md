### 🛍 Customer Lifecycle & Retention Analysis – UCI Online Retail Dataset
📖 Project Overview

This project analyses customer behaviour and retention patterns using the UCI Online Retail Dataset (transactions from a UK-based e-commerce store). The goal was to understand how customer cohorts behave over time, identify key retention trends, and estimate customer lifetime value (CLV).

The work combines data wrangling, cohort analysis, retention visualisation, and customer segmentation to generate insights that can inform real-world marketing and growth strategies.

🧰 Tools & Technologies

Python: pandas, numpy, seaborn, matplotlib

SQL: for exploratory queries and frequency analysis

Power BI: for interactive dashboards

Excel: initial exploration and data cleaning

📊 Key Analyses
1. Cohort Analysis

Customers were grouped by their first purchase month (CohortMonth).
For each cohort, retention and revenue were tracked across monthly periods (CohortPeriod) to reveal how customer engagement evolved over time.

Outputs:

Customer Retention Heatmap – shows how many customers from each cohort remained active after 1, 2, 3… months.

Revenue Retention Heatmap – shows how much of the cohort’s original revenue was retained over time.

Insight Example:
Early cohorts showed a sharp revenue drop (around 60–70% loss by month 3), stabilising around 15–30% for mature cohorts — indicating a small group of loyal customers driving consistent revenue.

2. Purchase Frequency Analysis

A distribution of the number of purchases per customer highlighted the dominance of one-time buyers, but also revealed a smaller, valuable segment of repeat and loyal buyers.
This suggests strong potential for retention campaigns focused on re-engaging first-time customers.

3. Customer Segmentation & Lifecycle Metrics

Customers were segmented into:

New Customers: first-time buyers in the month

Repeat Customers: made 2–4 purchases

Loyal Customers: made 5+ purchases

Metrics calculated:

30-, 60-, 90-day retention

Average purchase frequency

Customer Lifetime Value (CLV) approximation

📈 Power BI Dashboard

The final dashboard (built in Power BI) visualises:

Cohort retention heatmaps

Customer lifecycle funnel

Purchase frequency distribution

Monthly revenue trends

Customer segmentation metrics

This interactive dashboard allows stakeholders to explore how acquisition, retention, and revenue interact over time.

📂 Project Structure
Customer_Lifecycle_Analysis/
│
├── data/
│   ├── processed/
│   │   ├── cohort_revenue_retention.csv
│   │   └── customer_summary.csv
│   └── (link to dataset on UCI repository)
│
├── notebooks/
│   └── customer_retention_analysis.ipynb
│
├── visuals/
│   ├── cohort_retention_heatmap.png
│   └── purchase_frequency_histogram.png
│
├── PowerBI_Dashboard.pbix
│
└── README.md

📚 Data Source

UCI Machine Learning Repository – Online Retail Dataset
Transactions from a UK-based online retailer between Dec 2010 and Dec 2011.
Dataset link: UCI Online Retail

Note: The raw dataset is not included in this repository due to licensing terms. Only derived and processed files are shared.

💡 Key Takeaways

Most customers make only one purchase — retention is the main growth lever.

Revenue retention stabilises around 20–30% for mature cohorts, showing a loyal base.

Clear opportunity for targeted engagement and loyalty programs to lift repeat behaviour.

Cohort and lifecycle analyses are practical tools for understanding long-term customer value.

🧠 Skills Demonstrated

Data cleaning and transformation with pandas

Cohort and retention analysis techniques

Data visualisation with seaborn and Power BI

Deriving actionable business insights from customer data
