🛒 RetailMart SQL Analytics Dashboard

A complete end-to-end SQL-based analytics dashboard built using PostgreSQL 16 and a lightweight HTML-CSS-JS frontend.
This project showcases my ability to design a data model, write optimized SQL queries, create materialized views, build JSON APIs using SQL functions, and visualize insights through an interactive dashboard.

📌 Overview

RetailMart Analytics Dashboard provides insights across:

✔ Sales
✔ Product Performance
✔ Customer Behavior
✔ Store Performance

All analytics are fully generated through SQL functions and exported as JSON files, which the dashboard consumes dynamically.

📁 Project Structure
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
│   └── data/ (auto-generated JSON)
│
└── export_all_json.sh

✨ Key Features
🔹 Database Layer

17 SQL Views

8 Materialized Views

22 JSON Export Functions

Global refresh function

Metadata & audit tracking

🔹 Dashboard

Built using HTML, CSS, JavaScript (Chart.js)

Dynamic visualizations

KPI cards

Customer segmentation

Revenue trends

Real-time store & product insights

🔹 Automation

One-command JSON data export

Supports cron-based automated refresh

🚀 How to Run This Project
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

📊 Dashboard Sections
1. Executive Summary

Revenue

Orders

Customer Count

Top 10 Products

Monthly revenue trend

2. Sales Analytics

Daily performance

Category-wise revenue

Quarterly comparison

3. Product Performance

ABC Analysis

Top selling products

Product revenue share

4. Customer Insights

RFM segmentation

Customer Lifetime Value

Churn risk analysis

5. Store Performance

Top performing stores

Regional breakdown

Store scorecards

🎯 Skills

✔ SQL Views & Materialized Views
✔ PostgreSQL Functions (JSON Output)
✔ Data Modeling
✔ Performance Optimization
✔ Dashboard Development
✔ Shell Scripting (Automation)
✔ Analytics Communication
