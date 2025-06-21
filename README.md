# Financial-Analyzer-dashboard-
A Power BI dashboard project analyzing financial performance using the Superstore dataset. Includes KPIs, trends, regional insights, and interactive visuals.
🧰 Tools & Technologies Used

- Power BI Desktop
- Power Query
- DAX (Data Analysis Expressions)
- Excel (Data Source)


The dashboard consists of:

- ✅ KPI Cards: Total Sales, Total Profit, Profit Margin
- 📅 Line Chart: Monthly Sales & Profit Trends
- 🗺️ Map/Bar Charts: Sales by Region & State
- 📊 Category/Segment Breakdown
- 🔍 Interactive Filters: Region, Segment, Year

---

## 📐 Key DAX Measures

```DAX
Total Sales = SUM(Orders[Sales])
Total Profit = SUM(Orders[Profit])
Profit Margin = DIVIDE([Total Profit], [Total Sales])
Sales YOY Growth = 
    DIVIDE(
        [Total Sales] - CALCULATE([Total Sales], DATEADD(Orders[Order Date], -1, YEAR)),
        CALCULATE([Total Sales], DATEADD(Orders[Order Date], -1, YEAR))
    )
