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
- Generate pre-aggregated data models to power BI dashboards.
- Recommend data-driven vendor and product strategies.

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

- **📊 Vendor Profitability Comparison**  
  Bar chart comparing total revenue, cost, and net profit by vendor.

- **📉 Cost vs Selling Price Scatter Plot**  
  Identifies underpriced products with thin or negative margins.

- **📦 Freight Cost Distribution**  
  Histogram showing how freight charges vary among vendors.

- **📈 Gross Margin Analysis**  
  Vendor-wise margin per unit sold visualized using bar plots.

- **📊 Profitability Boxplots**  
  Highlights variability and outliers in vendor performance.

---

## 💡 Business Insights

- **Top vendors** deliver higher profit per unit and maintain lower freight rates.
- Certain products are priced too close to cost — opportunity for margin optimization.
- Pre-aggregated summaries significantly reduce dashboard load times and simplify reporting.

---

## ✅ Recommendations

- Prioritize vendors with the best net profit-to-cost ratio.
- Adjust pricing strategies for low-margin or loss-leading products.
- Set monthly automated refresh cycles for performance reporting.

### Author
Dhwani Zala
📧 dhwanizala25@gmail.com
