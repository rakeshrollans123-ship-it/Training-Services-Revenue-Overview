# Training Services – Revenue Overview (Power BI)

A Power BI dashboard giving a quick revenue overview for a training-services business that sells data and analytics courses. It tracks revenue, orders and customers by region, course and time period.

## What the Dashboard Shows
- **KPI cards:** Total Revenue, Total Customers, Total Orders
- **Revenue by Region** and **Revenue by Course** (bar charts)
- **Monthly Revenue Trend** and **Revenue by Quarter** (line charts)
- **Course × Region matrix** with revenue and order counts
- **Slicers:** Region and Year (2025 / 2026)

Courses analysed: Excel Analytics, GenAI for Business, Power BI Bootcamp, Python for Analytics, SQL Essentials.

## Data Model
Star schema:

| Table | Role |
|---|---|
| `Fact_Orders` | Order transactions |
| `Dim_Customer` | Customer attributes |
| `Dim_Course` | Course catalogue |
| `Dim_Region` | Regions |
| `Dim_Date` / `Dim_Date_calendar` | Date dimensions |
| `Targets` | Revenue targets |

## Tools
Power BI Desktop · DAX · Power Query

## How to Use
1. Download the `.pbix` file.
2. Open it in Power BI Desktop.
3. Use the Region and Year slicers to explore the data.

## Repository Contents
```
├── README.md
├── screenshots/dashboard.png    # dashboard preview
└── model-files/                 # internal Power BI model parts
    ├── DataModel
    ├── DiagramLayout
    ├── Metadata
    ├── SecurityBindings
    ├── Settings
    ├── Version
    └── [Content_Types].xml
```
