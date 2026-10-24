# Retail Sales Analysis & Business Intelligence Dashboard

**Tools:** Microsoft Power BI | Power Query | DAX | Data Modeling | Data Visualization

**Project Status:** In Progress

## Overview

This project aims to develop an interactive Business Intelligence dashboard using Microsoft Power BI to analyze retail sales performance and transform raw data into actionable business insights.

Using the Lotus Group Retail Star Schema BI dataset, the project explores data preparation, dimensional modeling, business KPI development, and interactive reporting.

The objective is to build a structured, reliable, and user-friendly analytical solution that supports retail business performance monitoring and decision-making.

## Business Objectives

- Analyze retail sales and revenue performance over time.
- Evaluate product and category performance.
- Compare sales performance across stores and regions.
- Explore customer segments and loyalty tiers.
- Analyze order statuses, payment methods, and returns.
- Develop KPIs to monitor business performance.
- Build interactive reports that allow users to explore data using filters and slicers.

The final analysis will depend on the available data and the validation of business definitions.

## Dataset

**Source:** [Lotus Group Retail Star Schema BI — Kaggle](https://www.kaggle.com/datasets/abdelrahmanmahmoud22/lotus-group-retail-star-schema-bi)

The dataset contains nine CSV files organized around retail transactions and their related business dimensions.

### Dataset Structure

| File | Purpose |
|---|---|
| `fact_orders_2022_2023.csv` | Order-level information for 2022–2023 |
| `fact_orders_2024.csv` | Order-level information for 2024 |
| `fact_order_details.csv` | Individual order lines, quantities, prices, discounts, revenue, and costs |
| `fact_returns.csv` | Return records, reasons, refund amounts, and statuses |
| `dim_products.csv` | Product attributes, categories, brands, prices, costs, and stock |
| `dim_customers.csv` | Customer attributes and loyalty information |
| `dim_stores.csv` | Store locations, regions, sizes, and types |
| `dim_employees.csv` | Employee information and store assignments |
| `dim_date.csv` | Calendar attributes for time-based analysis |

## Tools & Technologies

- **Power BI Desktop:** Report development and data modeling.
- **Power Query:** Data cleaning, transformation, and preparation.
- **DAX:** Business calculations, measures, and KPIs.
- **Dimensional Modeling:** Relationships between fact and dimension tables.
- **Data Visualization:** Interactive charts, tables, cards, and slicers.
- **GitHub:** Project documentation and version management.

## Planned Data Model

The project will use a dimensional modeling approach based on the dataset's existing star-schema structure.

The initial model will investigate the following logical tables:

- **FactOrders:** Order-level information, combining the two yearly order files after schema validation.
- **FactOrderDetails:** Product-level order line information.
- **FactReturns:** Records of returned orders and refund information.
- **DimDate:** Calendar attributes.
- **DimProducts:** Product descriptions and classifications.
- **DimCustomers:** Customer attributes and loyalty tiers.
- **DimStores:** Store and geographic information.
- **DimEmployees:** Employee and store assignment information.

Relationships, table grain, key uniqueness, and filter direction will be validated before finalizing the model. The relationship between orders and order details, in particular, must be designed carefully to avoid duplicated calculations.

## Planned KPIs

Subject to data validation and clearly defined business rules, the dashboard may include:

- Total Revenue
- Total Orders
- Units Sold
- Average Order Value
- Total Cost
- Gross Profit
- Gross Profit Margin
- Sales Growth
- Return Rate
- Revenue by Product Category
- Revenue by Store and Region
- Sales Trends Over Time

Each KPI will be defined and validated before implementation.

## Implementation Roadmap

- [ ] Inspect the dataset and understand its structure.
- [ ] Audit data quality, missing values, and key uniqueness.
- [ ] Clean and transform data using Power Query.
- [ ] Combine the order tables where appropriate.
- [ ] Build and validate the dimensional data model.
- [ ] Develop DAX measures and business KPIs.
- [ ] Design interactive report pages.
- [ ] Validate calculations against the source data.
- [ ] Optimize the report and improve usability.
- [ ] Publish and document the appropriate sharing method.
- [ ] Add dashboard screenshots and business insights.

## Repository Structure

```text
retail-sales-analysis-powerbi/
├── README.md
├── powerbi/
│   └── lotus retail.pbix
├── screenshots/
│   ├── executive_overview.png
│   ├── product_analysis.png
│   └── sales_trends.png
└── documentation/
    ├── data_model.md
    └── business_insights.md
```

The files above represent the planned repository structure. Files will be added as the project progresses.

## Data Privacy

The source customer table contains contact information. Personal information will be excluded from public documentation and handled appropriately before publishing or distributing project files.

The original dataset will not be redistributed unless its applicable license and terms permit it.

## Expected Deliverables

- An interactive Power BI report.
- A documented and validated data model.
- Reusable DAX measures for retail performance analysis.
- Documentation of data preparation and analytical decisions.
- Dashboard screenshots and business insights.
- Instructions for accessing the published report, where applicable.

## Disclaimer

This is an independent educational portfolio project developed to practice Business Intelligence, data modeling, and retail analytics.
