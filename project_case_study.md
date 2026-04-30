# Project Case Study — Retail Sales Dashboard

## Overview
Retail businesses generate large volumes of transactional data, but decision‑makers often struggle to translate that information into clear, actionable insights. This project was created to solve that gap. I designed an interactive Power BI dashboard that transforms raw retail sales data into a visual, intuitive, and business‑focused analytics tool. The goal was to help stakeholders quickly understand performance trends, identify top‑selling products, compare regional results, and monitor customer activity — all in one place.

The project demonstrates end‑to‑end analytical thinking: from understanding the business problem, to modeling the data, to building meaningful KPIs, to designing visuals that communicate insights clearly. It reflects my ability to approach a real‑world scenario the way an analyst would — by asking the right questions, structuring the data effectively, and presenting insights that support decision‑making.

## Business Problem
Retail organizations rely on timely, accurate insights to make decisions about inventory, marketing, staffing, and product strategy. However, raw sales data alone doesn’t provide the clarity needed to understand performance or identify opportunities. Without a structured analytics solution, teams struggle to answer essential questions such as:

- Which products generate the most revenue?
- How do sales vary across regions?
- Are customer numbers increasing or declining?
- What trends are emerging over time?
- Which areas of the business require attention or investment?

This project addresses these challenges by transforming disconnected sales records into a unified, interactive dashboard. The goal is to give decision‑makers a clear view of performance, highlight patterns that may not be immediately obvious, and support data‑driven actions that improve business outcomes.

## Data & Modeling
The dataset includes sales transactions, product information, customer details, and date fields. To support accurate analysis, I structured the data using a simple star schema:

- **Fact Table:** Sales  
- **Dimension Tables:** Products, Customers, Calendar  

Relationships were created on Product, CustomerID, and Date to ensure proper filtering and time‑intelligence behavior. This model enables flexible slicing across products, regions, and time periods.

## DAX Measures
To support KPI calculations and visual insights, I created several core DAX measures:

```DAX
Total Sales = SUM('Sales'[Sales])

Total Quantity = SUM('Sales'[Quantity])

Total Customers = DISTINCTCOUNT('Sales'[CustomerID])

Total Products Sold = DISTINCTCOUNT('Sales'[Product])
```

These measures form the foundation of the dashboard’s performance indicators and trend analysis.

## Dashboard Design
The dashboard was designed with clarity and usability in mind. It includes:

### Top KPIs
- Total Sales  
- Total Customers  
- Total Quantity  
- Total Products Sold  

These metrics provide an immediate snapshot of business performance.

### Trend Analysis
A line chart visualizes Sales YTD over time, helping stakeholders identify seasonal patterns, growth trends, and anomalies.

### Category & Regional Insights
- **Top Products by Sales** highlights high‑performing items.
- **Sales by Region** compares geographic performance.
- **Total Sales by Month** reveals monthly fluctuations and patterns.

The layout prioritizes readability, consistent formatting, and intuitive navigation.

## Key Insights
From the analysis, several insights emerged:

- Sales show clear seasonal patterns across months.
- A small set of products drive a significant portion of total revenue.
- Regional performance varies, indicating opportunities for targeted strategies.
- Customer volume and quantity sold align closely with revenue trends.

These insights help guide decisions around inventory planning, marketing focus, and resource allocation.

## Conclusion
This project demonstrates my ability to take a real‑world business problem, structure the data effectively, build meaningful metrics, and design a dashboard that communicates insights clearly. It showcases skills in data modeling, DAX, visualization design, and analytical storytelling — all essential for delivering value as a data analyst.
