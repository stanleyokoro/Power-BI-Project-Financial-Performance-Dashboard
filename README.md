# 💼 Power BI Project – Financial Performance Dashboard

This project presents an end-to-end financial performance analysis dashboard built with Microsoft Power BI. The dashboard tracks key financial metrics across regions, products, and customer segments using a well-modeled dataset and dynamic DAX calculations. The result is a visually compelling and insightful report that supports strategic decision-making.

---

## 📘 Project Overview

The dataset (`financials`) includes the following columns:

- `Units Sold`
- `Sale Price`
- `Discounts`
- `Manufacturing Price`
- `Country`

The primary goal of this project is to:

- Monitor business performance using financial KPIs
- Evaluate profitability across countries and segments
- Understand the effects of discounts on net sales
- Recommend strategic improvements for underperforming areas

---

## 🧠 DAX Measures Used

DAX was used extensively to create customized calculations for KPIs, conditional formatting, and performance analysis.

| Measure                | Description |
|------------------------|-------------|
| `Total Transactions`   | Total number of transactions (rows) |
| `Canada Transactions`  | Transactions filtered for Canada |
| `COGS`                 | Cost of Goods Sold |
| `Gross Sales`          | Units Sold × Sale Price |
| `Total Discount`       | Sum of all discounts |
| `Net Sales`            | Gross Sales – Total Discount |
| `Total Profit`         | Net Sales – COGS |
| `Profit Positive`      | Displays only profits (values > 0) |
| `Profit Negative`      | Displays only losses (values < 0) |
| `Conditional Formatting` | Colors for profit vs loss (Purple/Red) |

➡️ See the [`/dax-measures/financial-kpis.dax`](./dax-measures/financial-kpis.dax) file for full definitions.

---

## 📊 Dashboard Insights

### 🔹 Summary (France)

| Metric                  | Value     |
|-------------------------|-----------|
| Total Transactions      | 140       |
| Total Quantity Sold     | 241K      |
| Gross Sales             | £26M      |
| Net Sales               | £24M      |
| COGS                    | £23M      |
| Total Discount          | £2M       |
| Total Profit            | £2M       |

![France Analysis](./assets/profit-analysis-france.png)

---

## 🔍 Key Analytical Insights

### ✅ Performance Monitoring
- Profitability evaluated using **Net Sales**, **COGS**, and **Total Profit**
- Conditional formatting helps quickly differentiate between profit/loss

### 🌍 Country Comparison
- **Germany** is top-performing with £3.26M in profit
- **France** underperforms with £1.82M in profit  
> 📌 *Action:* Benchmark Germany’s strategies to improve France’s profitability

### 🧩 Segment Profitability

| Segment         | Profit    |
|-----------------|-----------|
| Small Business  | £4.8M ✅ |
| Enterprise      | £1.8M     |
| Government      | £1.4M     |
| Channel Partners| -£2.9M ❌ |
| Midmarket       | -£3.4M ❌ |

> 🔍 Focus on restructuring Midmarket and Channel Partner business models

### 🏷️ Discount Analysis

| Discount Band | Profit     |
|---------------|------------|
| Low           | £3.0M ✅  |
| Medium        | £2.4M      |
| None          | -£0.4M     |
| High          | -£3.1M ❌  |

> 📌 *Action:* Reduce high discounting to improve profit margins

### 📅 Time-Based Trends

- **Monthly:** Decline from May–August; recovery begins October
- **Weekday:** Highest profit on Wednesdays and Saturdays; lowest on Sundays and Tuesdays
- **Yearly:** 2014 accounts for 94.8% of total profit vs 2013

---

## 🎯 Strategic Recommendations

- 🔄 **Refactor Segments**: Focus on loss-making segments (Midmarket & Channel Partners)
- 🎯 **Optimize Discounts**: Use low-medium discounts for better profitability
- 📅 **Boost Low Days**: Improve Sunday and Tuesday performance through campaigns
- 📍 **Leverage Winners**: Replicate successful strategies from Germany in lower-performing regions

---

## 🛠 Tools & Technologies

- **Power BI Desktop**
- **DAX (Data Analysis Expressions)**
- **Data Modeling (Star Schema)**
- **Power Query for data transformation**
- **Custom Visuals & Conditional Formatting**

---

## 📂 Repository Structure

```bash
financial-performance-dashboard-powerbi/
│
├── assets/                        # Visuals & Screenshots
│   └── profit-analysis-france.png
│
├── dax-measures/
│   └── financial-kpis.dax        # All DAX logic used in the dashboard
│
├── pbix/
│   └── financial-dashboard.pbix  # Power BI file (if sharable)
│
├── README.md                     # Main documentation
└── LICENSE                       # Project license (MIT or other)
```

---

## 🙋‍♂️ Author

**Stanley Chinor Okoro**  
📧 stanley.chinor@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/timelesshov) | [GitHub](https://github.com/timelesshov)

---

## ⭐️ Like This Project?

If this project helped or inspired you, feel free to give it a ⭐ on GitHub. Feedback is welcome!
