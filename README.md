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
- Identify Brands that needs Promotional or Pricing Adjustments Which exhibit lower sales performance but higher profit margins.

---

## 🔍 Data Overview

Key tables used from the SQLite database:

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

- Joins multiple tables into a unified `vendor_sales_summary` dataframe.
- Computes:
  - **Total Purchase Cost**
  - **Sales Revenue**
  - **Freight Charges**
  - **Net Profit** = Revenue − Cost − Freight
- Statistical testing using **T-tests** to evaluate vendor performance.
- Visual analysis for pricing, margins, and freight impact.

---

## 📊 Visualizations

The project includes several key visual analyses:

- **📊 Top 10 Vendors by Sales & Top 10 Brands by Sales**  
 
- **📉 Pareto Chart: Vendor Contribution to Total Purchases**  

- **📦 Impact Of Bulk Purchasing On Unit Price**  

- **📈 Confidence Interval Comparison: To vs.Low Vendors (Profit Margin)**  

- **📊 Profitability Boxplots**  

---
## Research Question Solved 
1. Identify Brands that needs Promotional or Pricing Adjustments Which exhibit lower sales performance but higher profit margins.
2. Which vendors and brands demonstrate the highest sales performance?
3. Which Vendors contribute the most to total purchase dollars?
4. How much of total procurement is dependent on the top vendors?
5. Does purchasing in bulk reduce the unit price, and what is the optimal purchase volume for cost savings?
6. Which vendors have low inventory turnover, indicating excess stock and slow-moving products?
7. How much capital is locked in unsold inventory per vendor, and which vendors contribute the most to it?
8. What is the 95% confidence intervals for profit margins of top-performing and low-performing vendors.
9. Is there a significant difference in profit Targins between top-performing and low-performing vendors?

## 💡 Business Insights

- **Top vendors** deliver higher profit per unit and maintain lower freight rates.
- Certain products are priced too close to cost — opportunity for margin optimization.
- Pre-aggregated summaries significantly reduce dashboard load times and simplify reporting.

---

## ✅ Recommendations

- Prioritize vendors with the best net profit-to-cost ratio.
- For High-Performing Vendors: If they aim to improve profitability, they could explore selective price adjustments, cost optimization, or bundling strategies.
- For Low-Performing Vendors: Despite higher margins, their low sales volume might indicate a need for better marketing, competitive pricing, or improved
distribution strategies.

### Author
Dhwani Zala
📧 dhwanizala25@gmail.com
