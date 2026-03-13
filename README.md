# customer-shopping-behavior-analysis
Customer segmentation and revenue analysis using Python (Pandas), SQL, and Power BI dashboard visualization.



## Summary

This project analyzes customer purchasing behavior and applies segmentation techniques to identify high-value and at-risk customers.

An end-to-end workflow was implemented:

**Python (data cleaning) → PostgreSQL (SQL analysis & RFM scoring) → Power BI (dashboard visualization)**

The goal is to derive actionable insights into revenue contribution and customer performance.



## Business Objective

- Identify high-value customer segments  
- Analyze revenue contribution by segment  
- Support retention and targeted marketing strategies  



## Tools & Technologies

- **Python (Pandas)** – Data cleaning   
- **PostgreSQL (SQL)** – CTEs, Aggregations, Window Functions
- **Power BI** – Dashboard visualization  


## Data Preparation

Data was cleaned in Python using Pandas:

- Missing value handling  
- Duplicate removal  
- Column standardization  
- Data type validation  

The cleaned dataset was programmatically inserted into PostgreSQL using `psycopg2` for structured SQL-based analysis.



## SQL Segmentation Approach

Customer-level metrics calculated:

- Total Orders  
- Total Revenue (Monetary)  
- Average Order Value  
- Lifetime Purchase Frequency  

Customers were scored using `NTILE(5)` to create:

- Frequency Score  
- Monetary Score  

Combined scores were used to segment customers into:

- Champions  
- Loyal  
- Potential  
- At Risk  



## Dashboard Overview

The Power BI dashboard highlights:

- Revenue by Segment  
- Customer Count by Segment  
- KPI Cards (Total Revenue, Customers, Avg Order Value)  
- Avg Revenue per Customer (Tooltip Metric)  

**[Dashboard Preview]**<img width="1050" height="574" alt="Screenshot 2026-03-12 at 10 02 21 PM" src="https://github.com/user-attachments/assets/f769d08d-952d-4bb9-8ae9-0847fee12542" />





## Key Insights

- Loyal customers generate the highest overall revenue.
- Revenue contribution differs significantly across segments.
- Mid-tier segments represent growth opportunities.
- Segmentation enables targeted retention strategies.


