# 📊 Vendor Performance & Product Pricing Optimization

This repository contains a complete data analysis workflow focused on evaluating vendor performance and optimizing product pricing using transactional data from an SQLite database.

---

## 📁 Project Files

- **`Exploratory Data Analysis.ipynb`**  
  Combines purchase, sales, and inventory data to produce a vendor-level performance summary.

- **`Vendor Performance Analysis.ipynb`**  
  Performs detailed statistical and visual analysis of vendor profitability, cost margins, and freight expenses.

- **`inventory.db`** *(Required)*  
  Local SQLite database containing normalized data on purchases, sales, inventory, and vendor invoices.

---

## 🎯 Project Objectives

- Evaluate vendor profitability and freight efficiency.
- Analyze selling price vs purchase cost to optimize margins.
- Identify brands that need promotional or pricing adjustments—those with lower sales but higher profit margins.

---

## 🔍 Data Overview

| Table             | Description                               |
|------------------|-------------------------------------------|
| `purchases`       | Vendor and brand-level purchase history   |
| `sales`           | Product-wise quantity and revenue data    |
| `purchase_prices` | Purchase cost per product per vendor      |
| `vendor_invoice`  | Vendor-level invoice and freight charges  |
| `begin_inventory` | Opening inventory by product              |
| `end_inventory`   | Closing inventory by product              |

---

## ⚙️ Methods & KPIs

- Merged multiple tables into a unified `vendor_sales_summary` dataframe.
- Key metrics computed:
  - **Total Purchase Cost**
  - **Sales Revenue**
  - **Freight Charges**
  - **Net Profit** = Revenue − Cost − Freight
- Performed **T-tests** for comparing vendor performance.
- Generated visualizations for pricing, margins, and freight impact.

---

## 📊 Visualizations

- **Top 10 Vendors by Sales & Top 10 Brands by Sales**
- **Pareto Chart: Vendor Contribution to Total Purchases**
- **Impact of Bulk Purchasing on Unit Price**
- **Confidence Interval Comparison: Top vs. Low Vendors (Profit Margin)**
- **Profitability Boxplots**

---

## ❓ Research Questions Answered

1. Which brands need promotional or pricing adjustments?
2. Which vendors and brands show the highest sales performance?
3. Who contributes most to total purchase dollars?
4. How dependent is procurement on the top vendors?
5. Does bulk purchasing reduce unit price? What's the optimal volume?
6. Which vendors have low inventory turnover?
7. How much capital is locked in unsold inventory by vendor?
8. What are the 95% confidence intervals for vendor profit margins?
9. Is there a significant difference in profit margins between top and low-performing vendors?

---

## 💡 Business Insights

- **Top vendors** show higher unit profit and lower freight rates.
- Certain products have prices too close to cost—margin improvement opportunity.
- Pre-aggregated data boosts dashboard performance and simplifies reporting.

---

## ✅ Recommendations

- Prioritize vendors with the highest net profit-to-cost ratio.
- **High-performing vendors**: Explore selective price increases or bundling.
- **Low-performing vendors**: Focus on marketing, competitive pricing, or better distribution.

---

## 👩‍💻 Author

**Dhwani Zala**  
📧 [dhwanizala25@gmail.com](mailto:dhwanizala25@gmail.com)

---
