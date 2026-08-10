# 🛒 Retail Sales — Exploratory Data Analysis

![Python](https://img.shields.io/badge/Python-3.8+-blue) ![Pandas](https://img.shields.io/badge/Pandas-2.0-green) ![Matplotlib](https://img.shields.io/badge/Matplotlib-Seaborn-orange) ![Status](https://img.shields.io/badge/Status-Completed-green)

## 🎯 Project Overview

Performed end-to-end Exploratory Data Analysis on a retail
sales dataset using Python. Analysed customer behaviour,
revenue trends, product performance and branch-level metrics
to extract actionable business insights.

---

## 📁 Project Structure
sales-eda-analysis/
│
├── eda.ipynb ← Main analysis notebook
├── sales.csv ← Raw dataset
└── README.md
---

## 🔍 Analysis Performed

### 📅 Time Analysis
- Monthly revenue trend (see note on synthetic dates below)
- Quarterly revenue comparison
- Peak and low revenue periods identified

### 🏷️ Product Analysis
- Revenue by product category
- Top 10 products by revenue
- Average order value by category

### 👥 Customer Analysis
- Member vs Normal customer comparison, tested for statistical significance
- Gender × Category revenue heatmap
- Reward points analysis

### 🏢 Branch & City Analysis
- Revenue by branch
- City-wise performance comparison
- Correlation matrix of numeric variables

---

## ⚠️ Note on Order_date

The source dataset (`sales.csv`) does not include an order date field.
To demonstrate time-series analysis technique, dates were synthetically
generated (`np.random.seed(42)`) and randomly assigned across 2024.

**As a result:** the Monthly Revenue Trend and Quarterly Comparison sections
in the notebook illustrate the *method* for time-series analysis, not real
seasonal patterns in this business. "Peak month" or "low month" findings
from this dataset are not treated as real insights below — see the
Key Insights table.

---

## 💡 Key Insights

| # | Insight | Action |
|---|---------|--------|
| 1 | Branch A handles 67% of orders and 70% of revenue | Investigate why Branch B underperforms — staffing, footfall, or product mix |
| 2 | Personal Care & Fruits account for 45% of revenue | Prioritise stock and shelf space for these categories |
| 3 | Members spend ~7% more per order than Normal customers, but the gap is **not statistically significant** (t-test, p = 0.20, n = 1000) | Don't act on this yet — flag for a larger sample or a controlled test before investing in a membership campaign |
| 4 | Chicago leads all cities in revenue | Investigate what's driving it before assuming it's replicable — could be store size, location, or customer base rather than "strategy" |

---

## 🛠️ Tools Used

| Tool                   | Purpose                        |
| ----------------------- | -------------------------------- |
| Python (pandas, numpy)  | Data manipulation                |
| Matplotlib               | Charts and visualisations        |
| Seaborn                  | Heatmaps and statistical plots   |
| SciPy                    | Significance testing             |
| Jupyter Notebook         | Analysis environment             |

---
## 🚀 How to Run

1. Clone this repo:
2. Install dependencies:
3. Open the notebook:

## 👩‍💻 Author

**Raghavi Gowda**
[GitHub](https://github.com/Raghavi-gowda)
