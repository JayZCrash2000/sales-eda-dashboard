# Sales EDA Dashboard

End-to-end exploratory data analysis on a retail sales dataset covering 2022-2024. Includes data cleaning, trend analysis, category and regional performance, discount impact analysis, and business insights.

---

## Problem Statement

Retail businesses generate large volumes of transactional data but rarely extract structured insights from it. This project demonstrates a full EDA pipeline that answers key business questions:

- Which categories and regions drive the most revenue and profit?
- How do discounts impact profitability?
- What are the seasonal trends quarter-over-quarter?
- Where are the margin risks?

---

## Tech Stack

- **Python** — Pandas, NumPy
- **Visualization** — Matplotlib, Seaborn
- **Environment** — Jupyter / Google Colab

---

## Project Structure

```
sales-eda-dashboard/
│
├── sales_eda_dashboard.ipynb   # Full EDA notebook
├── requirements.txt
└── README.md
```

---

## Dataset Overview

| Property | Value |
|---|---|
| Records | 2,000 orders |
| Date Range | 2022-01-01 to 2024-12-31 |
| Total Sales | ~3,190,644 |
| Total Profit | ~563,105 |
| Avg Profit Margin | 17.7% |
| Null Values | None |
| Duplicates | None |

---

## Analysis Sections

1. **Data Quality Check** — shape, nulls, duplicates, date range, summary stats
2. **Sales Trend Analysis** — monthly revenue and profit bar/line charts (2022-2024)
3. **Category Performance** — total sales and avg profit margin by product category
4. **Regional Analysis** — sales share across North, South, East, West, Central
5. **Customer Segment Analysis** — Consumer vs Corporate vs Home Office
6. **Discount Impact** — scatter plot and bucketed margin analysis by discount tier
7. **Quarterly YoY Comparison** — Q1-Q4 revenue comparison across 2022, 2023, 2024
8. **Correlation Heatmap** — relationships between quantity, price, discount, sales, profit

---

## Key Findings

**Revenue**
- Electronics is the highest revenue category, driven by high unit prices
- Q4 consistently outperforms other quarters — strong seasonal demand
- Revenue shows an upward YoY trend from 2022 to 2024

**Profitability**
- Grocery has the highest profit margin despite low unit prices — high volume, low discounting
- Discounts above 20% consistently destroy margin — profit turns negative at high discount tiers
- Corporate segment generates the highest absolute profit

**Regional Performance**
- Sales are evenly distributed across all five regions (~20% each)
- Regional strategy should focus on margin improvement, not just revenue growth

**Risk Flags**
- Discount rates above 20% on Furniture and Automotive are eroding margins
- Some months show negative profit — likely linked to aggressive seasonal discounting

**Recommendations**
1. Cap discounts at 15% across all categories to protect margins
2. Double down on Electronics + Corporate segment — highest revenue and profit combination
3. Investigate loss-making months for root cause (discount spikes vs demand drops)
4. Expand Same Day shipping for high-margin Electronics orders to improve customer satisfaction

---

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook sales_eda_dashboard.ipynb
```

---

## Author

**Jeet Kumar** — [GitHub](https://github.com/JayZCrash2000) | [LinkedIn](https://linkedin.com/in/YOUR_LINKEDIN)
