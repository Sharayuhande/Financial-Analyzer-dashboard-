# Financial-Analyzer-dashboard-
A Power BI dashboard project analyzing financial performance using the Superstore dataset. Includes KPIs, trends, regional insights, and interactive visuals.
🧰 Tools & Technologies Used

- Power BI Desktop
- Power Query
- DAX (Data Analysis Expressions)
- Excel (Data Source)


## 📁 Dataset

The project uses the **Superstore Dataset**, which contains fictional retail data including:

- Orders
- Returns
- Sales
- Profits
- Customer segments
- Regions & categories

---

## 🛠️ Project Steps

### 1. Data Import
- Loaded Excel data into Power BI from the Superstore dataset.

### 2. Data Cleaning
- Removed nulls and duplicates
- Standardized column names
- Converted data types (e.g., dates, currency)

### 3. Data Modeling
- Created relationships between Orders, Returns, and Region tables
- Built a star schema for efficient analysis

### 4. Measures (DAX)
Key measures created:
```DAX
Total Sales = SUM(Orders[Sales])
Total Profit = SUM(Orders[Profit])
Profit Margin = DIVIDE([Total Profit], [Total Sales])

