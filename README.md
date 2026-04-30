# Retail Sales Dashboard — Power BI Project

## Overview
This project is an interactive Power BI dashboard designed to analyze retail sales performance across products, regions, and time. It provides a clear view of business trends through KPIs, time‑series analysis, and category breakdowns. The goal is to help stakeholders quickly understand sales performance, customer behavior, and product trends.

## Business Problem
Retail managers need a simple, visual way to answer key questions:
- How much revenue are we generating?
- Which products drive the most sales?
- Which regions perform best?
- How do sales trend over time?
- Are we gaining or losing customers?

This dashboard solves that by turning raw CSV data into actionable insights.

## Dataset Description
The dataset includes:
- Sales transactions
- Product information
- Customer data
- Dates and time periods

Key fields used:
- OrderDate
- Product
- Region
- Quantity
- Sales
- CustomerID

## Data Model
A simple, clean star‑style model:

- **Fact Table:** Sales  
- **Dimension Tables:** Products, Customers, Calendar  

Relationships were created on Product, CustomerID, and Date to ensure accurate filtering and time‑intelligence calculations.

## DAX Measures

```DAX
Total Sales = SUM('Sales'[Sales])

Total Quantity = SUM('Sales'[Quantity])

Total Customers = DISTINCTCOUNT('Sales'[CustomerID])

Total Products Sold = DISTINCTCOUNT('Sales'[Product])
```

## Dashboard Visuals
The dashboard includes:

### Top KPIs
- Total Sales  
- Total Customers  
- Total Quantity  

### Trend Visual
- Sales YTD by Date (line chart)

### Category and Regional Insights
- Top Products by Sales  
- Sales by Region  
- Total Sales by Month  

## Key Insights
- Sales show clear seasonal patterns across months  
- A small set of products drive the majority of revenue  
- Regional performance varies significantly  
- Customer volume and quantity sold align with revenue trends  

## Tools Used
- Power BI Desktop  
- DAX  
- Data Modeling  
- CSV Data Processing  

## Dashboard Screenshot
(Insert your screenshot after uploading to GitHub)

Example:
```markdown
![Retail Sales Dashboard](images/dashboard.png)
```

## How to Open the PBIX
1. Download the `.pbix` file from this repository  
2. Open it in **Power BI Desktop**  
3. Interact with slicers and visuals to explore insights  

## Project Summary
This project demonstrates:
- Data cleaning  
- Data modeling  
- DAX measure creation  
- Dashboard design  
- Insight communication  

It is designed as a portfolio‑ready Power BI project showcasing analytical and visualization skills.
