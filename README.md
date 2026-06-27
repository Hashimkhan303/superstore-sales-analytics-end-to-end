# 🏪 Superstore Sales Analysis — End-to-End Analytics Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=python&logoColor=white)

## 📌 Project Overview

This project delivers a **complete sales analysis** of the Superstore retail 
dataset using Python for data cleaning and exploratory analysis, plus an 
interactive Power BI dashboard.

The goal is to uncover **sales patterns, profitability drivers**, and provide 
**actionable business recommendations** to improve revenue and margins.

> 💡 **Business Context:** A US-based retail superstore is losing profit on 
> certain products and regions. This analysis identifies exactly where money 
> is being lost and what actions to take.

---

## 🎯 Business Questions Answered

| # | Question |
|---|---|
| 1 | Which products, categories, and regions drive the most revenue? |
| 2 | How do discounts impact profit margins? |
| 3 | What are the key sales trends over time? |
| 4 | Which states and customers are most valuable? |
| 5 | What actions can improve profitability? |

---

## 🔑 Key Findings

### By Category
| Category | Sales | Profit | Profit Margin |
|---|---|---|---|
| 💻 Technology | $836,154 | $145,455 | 17.4% |
| 📎 Office Supplies | $719,047 | $122,491 | 17.0% |
| 🪑 Furniture | $741,999 | $18,451 | **2.5%** ⚠️ |

### By Region
| Region | Sales | Performance |
|---|---|---|
| West | $725,458 | 🏆 Highest |
| East | $678,781 | 2nd |
| Central | $501,240 | Average |
| South | $391,722 | ❌ Lowest |

### Key Metrics
| Metric | Value |
|---|---|
| 💰 Total Sales | $2,297,201 |
| 📈 Total Profit | $286,397 |
| 📦 Total Orders | 5,009 |
| 📊 Profit Margin | 12.47% |

> 💡 **Key Insight:** Technology drives the highest profit while Furniture 
> (especially Tables & Bookcases) is dragging down overall profitability. 
> Discounts above 40% consistently result in losses.

---

## ⚠️ Discount Impact Analysis

| Discount Rate | Profit Impact |
|---|---|
| 0–20% | ✅ Positive profit |
| 20–40% | ⚠️ Reduced profit margins |
| 40%+ | ❌ Consistent losses |

> 📉 Correlation between Discount and Profit = **-0.22** (negative relationship)
> Higher discounts = lower profits

---

## 📈 Loss-Making Sub-Categories

| Sub-Category | Profit Status |
|---|---|
| Tables | ❌ -$17,725 (Loss) |
| Bookcases | ❌ -$3,473 (Loss) |
| Phones | ✅ $44,516 (Profit) |
| Copiers | ✅ $55,618 (Profit) |

---

## 🎯 Recommended Actions

### By Category
| Category | Recommended Action |
|---|---|
| Technology | Increase inventory before peak months, cross-promote accessories |
| Office Supplies | Maintain current strategy, optimize pricing |
| Furniture | Investigate losses, renegotiate supplier or increase price |

### By Issue
| Issue | Recommended Action |
|---|---|
| High Discount Losses | Cap discounts at 20–30% maximum |
| Low Furniture Profit | Bundle with profitable items or discontinue worst SKUs |
| Peak Season Demand | Increase inventory 30% before November–December |
| Low South Region | Replicate West region success factors |
| Top Customers | Launch loyalty program for top 10 customers |

---

## 🖥️ Dashboard Screenshots

### Power BI Dashboard
![Dashboard](Dashboard/Power%20BI%20Dashboard.png)

---

## 🔬 Methodology

### Step 1 — Data Cleaning
- Converted date columns to datetime format
- Checked for missing values (none found)
- Validated data types and distributions
- Created new features: Order Year, Order Month

### Step 2 — Exploratory Data Analysis
- Analyzed sales and profit by category, region, sub-category
- Examined monthly and yearly sales trends
- Investigated discount vs profit relationship
- Identified top 10 customers, products, and profitable states
- Created correlation heatmap (Sales, Profit, Discount, Quantity)

### Step 3 — Feature Engineering
- Extracted Order Year from Order Date
- Extracted Order Month from Order Date
- Grouped data for time series analysis

### Step 4 — Power BI Dashboard
- Built interactive dashboard with KPIs and filters
- KPI Cards: Total Sales, Profit, Orders, Margin
- Visuals: Sales trend, Sales by Category, Sales by Region
- Filters: Region, Category, Year

---

## 📊 Dataset

| Field | Detail |
|---|---|
| **Name** | Sample Superstore |
| **Source** | Kaggle / Tableau Superstore Dataset |
| **Type** | Retail sales transactions |
| **Period** | 2014 – 2017 |
| **Size** | 9,994 transactions |
| **Missing values** | None |

---

## 📁 Project Structure
superstore-sales-analytics/

│

├── 📂 Data/

│   ├── superstore_raw.csv

│   └── superstore_clean.csv

│

├── 📂 Notebooks/

│   └── sales_analysis.ipynb

│

├── 📂 Dashboard/

│   ├── SuperStore Sales Analysis Dashboard.pbix

│   └── Power BI Dashboard.png

│

├── requirements.txt

└── README.md
---

## 🕐 Time Trends

- **Peak months:** November – December (holiday season)
- **Lowest month:** February
- **Growth trend:** Steady increase from 2014 → 2017

---

## 👑 Top Customers

| Customer | Sales |
|---|---|
| Sean Miller | $25,043 |
| Tamara Chand | $19,052 |
| Raymond Buch | $15,117 |

---

## 🗺️ Top Profitable States

| State | Profit |
|---|---|
| California | $76,381 |
| New York | $74,039 |
| Washington | $33,403 |

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Python 3** | Data cleaning, EDA, feature engineering |
| **Pandas** | Data manipulation |
| **Matplotlib / Seaborn** | Visualizations in notebooks |
| **Google Colab** | Cloud-based Python environment |
| **Power BI** | Interactive dashboard |

---

## 🚀 How to Run

```bash
# Step 1: Clone the repository
git clone https://github.com/Hashimkhan303/superstore-sales-analytics

# Step 2: Install dependencies
pip install -r requirements.txt

# Step 3: Open notebook
jupyter notebook Notebooks/sales_analysis.ipynb
```

### Power BI Dashboard
1. Download `Dashboard/SuperStore Sales Analysis Dashboard.pbix`
2. Open in **Power BI Desktop** (free from Microsoft)
3. Refresh data if prompted
4. All visuals will load automatically

---

## 👨‍💻 Author

**Hashim Khan**

- 🐙 GitHub: [Hashimkhan303](https://github.com/Hashimkhan303)
- 💼 LinkedIn: ([paste your LinkedIn URL here](https://www.linkedin.com/in/hashim-khan-96b5082b4/))
- 🎓 Google Data Analytics Certificate
- 🎓 Google Advanced Data Analytics Certificate

---

## 📄 License

This project uses publicly available data from Kaggle.
Built for educational and portfolio purposes only.

---

⭐ **If you found this project useful, please give it a star!**
