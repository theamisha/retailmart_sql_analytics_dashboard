# Retailmart Analytics Project

This project provides analytics and dashboarding for Retailmart data, including customer, product, sales, and store analytics. It includes SQL scripts for schema setup, KPI queries, and a web-based dashboard for data visualization.

## Project Structure

- `01_setup/`: SQL scripts to set up analytics schema and metadata tables.
- `02_kpi_queries/`: SQL queries for key performance indicators (KPIs) across customers, products, sales, and stores.
- `03_dashboard/`: Web dashboard (HTML, JS, CSS) and JSON data files for visualizations.
- `04_documentation/`: Documentation including data dictionary and KPI definitions.
- `export_all_json.sh`: Script to export all analytics data to JSON.

## Usage

1. **Database Setup**
   - Run scripts in `01_setup/` to create the necessary schema and tables in your database.
2. **KPI Queries**
   - Execute queries in `02_kpi_queries/` to generate analytics data.
3. **Dashboard**
   - Open `03_dashboard/index.html` in a browser to view the analytics dashboard.
   - Data visualizations are powered by the JSON files in `03_dashboard/data/`.

## Git Commands

Typical workflow:

```sh
git add .
git commit -m "Your commit message"
git push
```

## License

Specify your license here.
