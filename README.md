# Commercial Performance & Potential Analysis
Power BI dashboard for analyzing sales performance, tracking plans and forecasts, and identifying growth opportunities across products, managers, and customers.
The project covers the full reporting process, from data preparation in Power Query to data modeling and DAX calculations.

<img width="1521" height="851" alt="Снимок экрана 2026-09-30 204436" src="https://github.com/user-attachments/assets/ae8bf8cc-401f-4432-bd1b-450832c7b81f" />

## Project Overview
The report brings together actual sales, sales plans, forecasts, and customer potential in one place. It allows users to compare performance across different periods, products, managers, and territories, and explore where sales are below potential. The dashboard includes several pages for overall performance, customer analysis, and product portfolio reporting.

## Data & Confidentiality
The report is based on a data snapshot from mid-August 2026. Automatic data refresh is not available because of confidentiality requirements under an NDA.
The published version is intended to demonstrate the data preparation process, data model, DAX calculations, and interactive reporting features. While the data is not up to date, the report illustrates the analytical approach, business logic, and trends visible in the available dataset.


## Data Preparation
Data was prepared and transformed using Power Query. The main steps included cleaning and restructuring source tables, changing data types, preparing dimension and fact tables, and organizing the data for reporting.

## Data Model
<img width="1402" height="801" alt="data-model" src="https://github.com/user-attachments/assets/8bf47e58-4e44-4ab6-a030-9fbc3bcc24ea" />
The report uses a star schema with two fact tables and several dimension tables.
Fact tables:
PF_2026 — actual sales, plans, and forecasts.
Potential — customer and market potential metrics.
Dimension tables:
Calendar
SKU
Managers
Territory
COMPANY
The tables are connected through one-to-many relationships with single-direction filtering.
A separate _Measures table is used to organize DAX calculations. The model also includes a Select Metric field parameter table for dynamic metric selection in the report.

## DAX & Analysis
The report uses DAX measures for sales performance analysis, time-based calculations, and comparisons between actual results, plans, forecasts, and potential.
The main calculations and features include:
Sales plan execution and forecast comparisons.
YTD sales and plan calculations.
Month-over-month sales growth.
Customer-level analysis of the gap between actual sales and potential.
Dynamic metric and chart dimension selection using Field Parameters.
Dashboard Features
The report includes interactive filters for products, product groups, managers, sectors, and territories.
Visuals include KPI cards, matrices with sparklines, treemaps, and combined column and line charts.
Users can switch between different metrics and dimensions to explore the data from different angles.

## Tools & Technologies
Power BI Desktop
Power Query
DAX
Star Schema Data Modeling
Field Parameters
Import Mode

## Files
- `Commercial_Performance.pbix` — Power BI report with data model, Power Query transformations, DAX measures, and report pages.
- `overview.png` — main dashboard.
- `data-model.png` — data model and relationships.
- `power-query.png` — data preparation and transformation steps.
