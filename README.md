# Superstore Sales Analysis Dashboard

**Tools:** Python | Pandas | Matplotlib | Seaborn | Power BI  
**Domain:** Retail Analytics | **Type:** End-to-End Analytics Project

---

## Project Overview

This project delivers a **complete sales analysis** of the Superstore dataset using Python for data cleaning and exploratory analysis, plus an interactive Power BI dashboard. The goal is to uncover sales patterns, profitability drivers, and provide actionable business recommendations.

The final output is an interactive Power BI dashboard that allows stakeholders to explore sales by category, region, product, and time period.

---

## Business Questions Answered

- Which products, categories, and regions drive the most revenue?
- How do discounts impact profit margins?
- What are the key sales trends over time?
- Which states and customers are most valuable?
- What actions can improve profitability?

---

## Dataset

**Name:** Sample Superstore  
**Source:** Kaggle / Tableau Superstore Dataset  
**Type:** Retail sales transactions  
**Period:** 2014 – 2017  
**Original Size:** 9,994 transactions  
**After Cleaning:** 9,994 transactions (no missing values)

| Column | Description |
|--------|-------------|
| Row ID | Unique row identifier |
| Order ID | Unique order identifier |
| Order Date | Date of purchase |
| Ship Date | Shipping date |
| Ship Mode | Shipping method |
| Customer ID | Unique customer identifier |
| Customer Name | Customer full name |
| Segment | Customer segment (Consumer, Corporate, Home Office) |
| Country | Customer country |
| City | Customer city |
| State | Customer state |
| Postal Code | Customer postal code |
| Region | Customer region (Central, East, South, West) |
| Product ID | Unique product identifier |
| Category | Product category (Furniture, Office Supplies, Technology) |
| Sub-Category | Product sub-category |
| Product Name | Full product name |
| Sales | Sales amount in USD |
| Quantity | Units purchased |
| Discount | Discount percentage applied |
| Profit | Profit amount in USD |

---

## Project Structure
superstore-sales-analytics-end-to-end/
│
\├── Data/
│ \├── superstore_raw.csv # Original dataset
│ \└── superstore_clean.csv # Cleaned & processed data
│
\├── Notebooks/
│ \└── sales_analysis.ipynb # Complete Python EDA
│
\├── Dashboard/
│ \├── SuperStore Sales Analysis Dashboard.pbix # Power BI file
│ \└── Power BI Dashboard.png # Dashboard preview
│
\├── .gitignore
\├── README.md
\└── requirements.txt

text

---

## Methodology

### Step 1 — Data Cleaning
- Converted date columns to datetime format
- Checked for missing values (none found)
- Validated data types and distributions
- Created new features: `Order Year`, `Order Month`

### Step 2 — Exploratory Data Analysis (EDA)
- Analyzed sales & profit by category, region, sub-category
- Examined monthly and yearly sales trends
- Investigated discount vs. profit relationship
- Identified top 10 customers, products, and profitable states
- Created correlation heatmap (Sales, Profit, Discount, Quantity)

### Step 3 — Feature Engineering
- Extracted `Order Year` from Order Date
- Extracted `Order Month` from Order Date
- Grouped data for time series analysis

### Step 4 — Power BI Dashboard
- Built interactive dashboard with KPIs and filters
- Page 1: Overview — Total Sales, Profit, Orders, Margin
- Visuals: Sales trend, Sales by Category, Sales by Region
- Filters: Region, Category, Year

---

## Key Findings

| Category | Sales | Profit | Profit Margin |
|----------|-------|--------|---------------|
| Technology | $836,154 | $145,455 | 17.4% |
| Office Supplies | $719,047 | $122,491 | 17.0% |
| Furniture | $741,999 | $18,451 | 2.5% |

| Region | Sales | Performance |
|--------|-------|-------------|
| West | $725,458 | Highest sales |
| East | $678,781 | Second highest |
| Central | $501,240 | Average |
| South | $391,722 | Lowest sales |

| Sub-Category | Profit Status |
|--------------|---------------|
| Tables | ❌ -$17,725 (Loss) |
| Bookcases | ❌ -$3,473 (Loss) |
| Phones | ✅ $44,516 (Profit) |
| Copiers | ✅ $55,618 (Profit) |

**Key Metrics:**
- Total Sales: **$2,297,201**
- Total Profit: **$286,397**
- Total Orders: **5,009**
- Profit Margin: **12.47%**

**Key Insight:** Technology drives highest profit while Furniture (especially Tables & Bookcases) is dragging down overall profitability. Discounts above 40% consistently result in losses.

---

## Discount Impact Analysis

| Discount Rate | Profit Impact |
|---------------|---------------|
| 0-20% | ✅ Positive profit |
| 20-40% | ⚠️ Reduced profit margins |
| 40%+ | ❌ Consistent losses |

**Correlation:** Discount vs Profit = **-0.22** (negative relationship)

---

## Time Trends

- **Peak months:** November – December (holiday season)
- **Lowest month:** February
- **Growth trend:** Steady increase from 2014 → 2017

---

## Top Customers

| Customer | Sales |
|----------|-------|
| Sean Miller | $25,043 |
| Tamara Chand | $19,052 |
| Raymond Buch | $15,117 |

---

## Top Profitable States

| State | Profit |
|-------|--------|
| California | $76,381 |
| New York | $74,039 |
| Washington | $33,403 |

---

## Recommended Actions by Category

| Category | Recommended Action |
|----------|---------------------|
| Technology | Increase inventory before peak months, cross-promote with accessories |
| Office Supplies | Maintain current strategy, optimize pricing |
| Furniture | Investigate Tables & Bookcases losses, consider supplier renegotiation or price increase |

---

## Recommended Actions by Segment

| Issue | Recommended Action |
|-------|---------------------|
| High Discount Losses | Cap discounts at 20-30% maximum |
| Low Furniture Profit | Bundle with profitable items or discontinue worst SKUs |
| Peak Season Demand | Increase inventory 30% before November-December |
| Low South Region Sales | Investigate and replicate West region success factors |
| Top Customers | Launch loyalty program for top 10 customers |

---

## Dashboard Screenshots

### Power BI Dashboard Preview
![Dashboard Preview](Dashboard/Power%20BI%20Dashboard.png)

**Dashboard Features:**
- KPI Cards: Total Sales ($2.30M), Profit ($286K), Orders (5,009), Margin (12.47%)
- Filters: Region, Category, Year
- Line Chart: Sales trend over time (2014-2017)
- Bar Charts: Sales & Profit by Category, Region, Product

---

## Tools and Technologies

| Tool | Purpose |
|------|---------|
| Python 3 | Data cleaning, EDA, feature engineering |
| Pandas | Data manipulation |
| Matplotlib / Seaborn | Visualizations in notebooks |
| Google Colab | Cloud-based Python environment |
| Power BI | Interactive dashboard |

---

## How to Run

1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Open `notebooks/sales_analysis.ipynb` in Jupyter or Google Colab
4. Run all cells in order
5. Open `Dashboard/SuperStore Sales Analysis Dashboard.pbix` in Power BI Desktop

### requirements.txt
pandas==1.5.3
numpy==1.24.3
matplotlib==3.7.1
seaborn==0.12.2
openpyxl==3.1.2

text

---

## Author

**Hashim Khan**  
Data Analyst | Python | SQL | Power BI .Machine Learning
Google Data Analytics Certificate | Google Advanced Data Analytics Certificate
