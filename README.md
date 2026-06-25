# Retail Sales Analysis
### Exploratory Data Analysis & Business Intelligence | Python · Power BI

> **Disclaimer:** This analysis is based on historical data from 2014–2017 and is intended for educational and portfolio purposes only.

---

## Project Overview

This project analyzes 4 years of retail transaction data from a U.S.-based superstore to answer real business questions around profitability, regional performance, seasonal trends, discount strategy, and customer value.

The analysis follows a structured business analytics workflow — from raw data exploration to actionable recommendations — simulating the kind of work a junior data analyst would deliver to management.

---

## Business Questions Answered

| # | Question |
|---|----------|
| 1 | Which product categories drive the most revenue vs profit? |
| 2 | Which sub-categories are loss-making despite high sales? |
| 3 | Which regions are underperforming on profitability? |
| 4 | What seasonal patterns exist in sales and profit? |
| 5 | How do discounts affect profit margins? |
| 6 | Which customers and products drive the most value? |

---

## Dataset

**Source:** Sample Superstore Dataset (Kaggle)  
**Period:** January 2014 – December 2017  
**Size:** 9,994 rows × 19 columns  

Key columns: `Order Date`, `Category`, `Sub-Category`, `Region`, `Sales`, `Profit`, `Discount`, `Customer ID`, `Product Name`

---

## Tools Used

- **Python** — Pandas, NumPy, Matplotlib, Seaborn
- **Jupyter Notebook** — Analysis & documentation
- **Power BI** — Interactive dashboard *(in progress)*

---

## Project Workflow & Key Findings

### 1. KPI Analysis

| Metric | Value |
|--------|------:|
| Total Sales | $2,297,200 |
| Total Profit | $286,397 |
| Profit Margin | ~12.5% |
| Total Orders | 5,009 |
| Total Units Sold | 37,873 |
| Avg. Order Value | ~$458 |

---

### 2. Category Analysis

| Category | Sales | Profit | Margin |
|----------|------:|-------:|-------:|
| Technology | $836,154 | $145,454 | 17.4% |
| Office Supplies | $719,047 | $122,490 | 17.0% |
| Furniture | $741,999 | $18,451 | 2.5% |

**Key Insight:** Furniture generates the second-highest revenue but has a critically low profit margin of just 2.5% — a major red flag requiring pricing and discount review.

---

### 3. Sub-Category Analysis

**Top Profit Performers:** Copiers, Phones, Accessories, Paper, Binders

**Loss-Making Sub-Categories:**

| Sub-Category | Status |
|-------------|--------|
| Tables | Highest loss |
| Bookcases | Loss-making |
| Supplies | Loss-making |

**Key Insight:** Tables rank 4th in sales but are one of the biggest loss-makers — a classic revenue-without-profit trap caused by excessive discounting.

---

### 4. Regional Analysis

| Region | Sales | Profit |
|--------|------:|-------:|
| West | Highest | Highest |
| East | 2nd | 2nd |
| Central | 3rd | Lowest |
| South | Lowest | 3rd |

**Key Insight:** Central region has strong sales but the lowest profit of all regions — suggesting over-discounting by regional sales teams.

---

### 5. Time Analysis

- Sales spike consistently between **October–January** every year (Q4 holiday + year-end buying)
- **2017** shows the strongest year-over-year growth
- **January 2015** recorded a significant profit loss despite post-holiday sales
- Most profitable sustained period: **July 2016 – April 2017**

---

### 6. Discount Analysis

- Average discount offered: **~15.6%**
- A significant cluster of orders carry **40–80% discounts** — these are almost certainly loss-making transactions
- Discount vs Profit correlation: **-0.22** (higher discounts consistently reduce profit)

---

### 7. Customer Analysis

- Top 10 customers by **Sales** and **Profit** identified separately
- Top profit customers ≠ top sales customers — high revenue does not always mean high profitability at the customer level
- Customers appearing in both lists represent the highest overall business value and should be prioritized for retention

---

### 8. Product Analysis

- **Canon imageCLASS 2200 Copier** is the top revenue-generating product by a significant margin
- Top 10 products dominated by high-ticket office equipment — confirming B2B purchasing patterns
- Top profit products and top sales products overlap but are **not identical** — revenue and margin are separate levers

---

## Business Recommendations

1. **Fix the Furniture problem** — Conduct a full pricing and discount audit on Tables and Bookcases. Either reprice or consider discontinuation.
2. **Protect Technology** — The only category winning on both revenue and profit. Prioritize inventory and marketing here.
3. **Cap discounts at 20%** — Orders with 40%+ discounts are loss-making. Implement a discount approval policy above this threshold.
4. **Investigate Central region** — High sales but lowest profit. Likely structural over-discounting by regional teams.
5. **Prepare for Q4 demand** — Sales spike Oct–Jan every year. Stock inventory and scale logistics 6–8 weeks in advance.
6. **Retain top customers** — High revenue concentration in a small group. A churn event here materially impacts the business.

---

## Skills Demonstrated

`Exploratory Data Analysis` · `Business KPI Analysis` · `Pandas & NumPy` · `Data Visualization` · `Time-Series Analysis` · `Discount Impact Analysis` · `Business Insight Generation` · `Data-Driven Recommendations`

---

## Future Enhancements

- [ ] Interactive Power BI Dashboard
- [ ] Customer Segmentation (RFM Analysis)
- [ ] Sales Forecasting with Machine Learning

---

## Project Structure

```
Retail-Sales-Analysis/
│
├── data/
│   └── sample_superstore_dataset.csv
├── notebooks/
│   └── retail_sales_analysis.ipynb
├── visuals/
│   └── (Power BI dashboard screenshots)
├── README.md
└── requirements.txt
```

---

## Author

**Yash**  
B.Sc. (Hons.) Computer Science — University of Delhi  
[GitHub](https://github.com/Yash-Codes07/retail-sales-analysis) · [LinkedIn](https://www.linkedin.com/in/yash-singh-ba9327375/)