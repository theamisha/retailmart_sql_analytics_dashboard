## **🛒 RetailMart SQL Analytics Dashboar**

A complete end-to-end SQL-based analytics dashboard built using PostgreSQL 16 and a lightweight HTML-CSS-JS frontend.
This project showcases my ability to design a data model, write optimized SQL queries, create materialized views, build JSON APIs using SQL functions, and visualize insights through an interactive dashboard.

## **📌 Overview**

RetailMart Analytics Dashboard provides insights across:

✔ Sales

✔ Product Performance

✔ Customer Behavior

✔ Store Performance

All analytics are fully generated through SQL functions and exported as JSON files, which the dashboard consumes dynamically.

## 📁 Project Structure

```
retailmart_analytics_project/
│
├── 01_setup/
│   ├── create_analytics_schema.sql
│   └── create_metadata_tables.sql
│
├── 02_kpi_queries/
│   ├── sales_analytics.sql
│   ├── product_analytics.sql
│   ├── customer_analytics.sql
│   └── store_analytics.sql
│
├── 03_dashboard/
│   ├── index.html
│   ├── dashboard.js
│   ├── styles.css
│   └── data/  (auto-generated JSON)
│
└── export_all_json.sh
```


## **✨ Key Features**

🔹 Database Layer
1. 17 SQL Views
2. 8 Materialized Views
3. 22 JSON Export Functions
4. Global refresh function
5. Metadata & audit tracking

🔹 Dashboard
1. Built using HTML, CSS, JavaScript (Chart.js)
2. Dynamic visualizations
3. KPI cards
4. Customer segmentation
5. Revenue trends
6. Real-time store & product insights

🔹 Automation
1. One-command JSON data export
2. Supports cron-based automated refresh

## **🚀 How to Run This Project**

1️⃣ Run SQL Setup

psql -U postgres -d retailmart -f 01_setup/create_analytics_schema.sql

psql -U postgres -d retailmart -f 01_setup/create_metadata_tables.sql

2️⃣ Load Analytics Modules

psql -U postgres -d retailmart -f 02_kpi_queries/sales_analytics.sql

psql -U postgres -d retailmart -f 02_kpi_queries/product_analytics.sql

psql -U postgres -d retailmart -f 02_kpi_queries/customer_analytics.sql

psql -U postgres -d retailmart -f 02_kpi_queries/store_analytics.sql

3️⃣ Export JSON Files

chmod +x export_all_json.sh

./export_all_json.sh refresh

4️⃣ Launch Dashboard
cd 03_dashboard

python3 -m http.server 8000


Visit:
👉 http://localhost:8000

## **📊 Dashboard Sections**
1. Executive Summary
A. Revenue
B. Orders
C. Customer Count
D. Top 10 Products
E. Monthly revenue trend

2. Sales Analytics
A. Daily performance
B. Category-wise revenue
C. Quarterly comparison

3. Product Performance
A. ABC Analysis
B. Top selling products
C. Product revenue share

4. Customer Insights
A. RFM segmentation
B. Customer Lifetime Value
C. Churn risk analysis

5. Store Performance
A. Top performing stores
B. Regional breakdown
C. Store scorecards

## **🎯 Skills**

✔ SQL Views & Materialized Views

✔ PostgreSQL Functions (JSON Output)

✔ Data Modeling

✔ Performance Optimization

✔ Dashboard Development

✔ Shell Scripting (Automation)

✔ Analytics Communication

## **📊 Dashboard Preview**

<img width="1918" height="968" alt="SQL_Dashboard" src="https://github.com/user-attachments/assets/04562094-1ee3-4004-ae12-4cd4e1dc0216" />


