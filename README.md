# Vendor Performance Analysis & Inventory Optimizatio

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)

## 📊 Power BI Dashboard
<img width="1376" height="764" alt="Screenshot (111)" src="https://github.com/user-attachments/assets/b2cdca05-81ae-4469-a5de-ce1d45ec2a40" />


## 📌 Project Overview
As a Data Analyst, I developed a comprehensive **Vendor Performance Analysis** model to help businesses optimize their inventory, track vendor performance, and maximize profit margins. This project bridges the gap between raw data and actionable business strategies by leveraging SQL for data transformation, Python for advanced exploratory data analysis (EDA), and Power BI for interactive visualization.

## 🛠️ Tech Stack & Methodology
- **SQL (SQLite):** Executed complex queries, multi-table joins, and aggregations (CTEs) across `purchases`, `sales`, `vendor_invoice`, and `purchase_prices` tables to engineer a comprehensive vendor summary dataset.
- **Python (Pandas, Matplotlib, Seaborn):** Conducted deep exploratory data analysis (EDA), data cleaning, and statistical correlation mapping. Derived key KPIs such as `GrossProfit`, `ProfitMargin`, `StockTurnover`, and `SalestoPurchaseRatio`.
- **Power BI:** Designed dynamic dashboards to visualize freight costs, vendor volume, sales vs. purchases, and profit metrics, providing a top-down view for stakeholders.

## 🎯 Problems Solved
1. **Disconnected Supply Chain Data:** Unified disparate sales, inventory, and freight data into a single source of truth (`vendor_sales_summary`).
2. **Hidden Logistics Costs:** Quantified the impact of freight costs on overall margin.
3. **Inventory Bottlenecks:** Calculated `StockTurnover` to identify products that are overstocked versus those selling efficiently.
4. **Vendor Profitability:** Identified which vendors drive the highest `Gross Profit` compared to those eating up capital with low ROI.

## 📈 Strategic Recommendations to Improve Sales & Profit

Based on the data insights generated in this project, here are actionable recommendations for the company:

### 1. Optimize Freight & Logistics
- **Insight:** High freight costs from certain vendors significantly erode profit margins.
- **Action:** Renegotiate shipping terms with high-freight vendors or explore local alternatives for bulky, low-margin items. Implement bulk-ordering for items with consistent demand to dilute freight cost per unit.

### 2. Double-Down on High-Turnover Vendors
- **Insight:** The `StockTurnover` ratio shows marked disparities between brands.
- **Action:** Direct more capital towards vendors supplying high-turnover products to avoid stockouts. For low-turnover stock, launch targeted promotional campaigns or bundle them with fast-moving goods to clear inventory and free up warehouse space.

### 3. Price Margin Adjustment (Gross Profit Focus)
- **Insight:** `SalestoPurchaseRatio` and `ProfitMargin` metrics reveal some products are selling at highly competitive rates but barely breaking even after excise taxes and purchasing costs.
- **Action:** Implement a dynamic pricing strategy. Marginally increase the price of highly inelastic (always in demand) goods where the current profit margin is sub-optimal. 

### 4. Vendor Consolidation
- **Insight:** The analysis inherently exposes bottom-performing vendors who yield the lowest total sales dollars relative to the purchase dollars invested.
- **Action:** Phase out underperforming vendor contracts. Consolidating volume with the top 20% of high-yield vendors can unlock volume discounts and better purchasing prices (economies of scale).

---

### 📂 Repository Contents
- **`Exploratory Data Analysis.ipynb`**: Extensive EDA notebooks showcasing data distributions, anomaly detection, and correlation matrices.
- **`Vendor Performance Analysis.ipynb`**: Deep dive notebook into the vendor KPIs.
- **`get_vendor_summary.py`**: Python script containing the SQL CTEs and Pandas transformation logic to generate our master analytical table.
- **`ingestion_db.py`**: Automated pipeline script for loading the cleaned data back into the database for BI consumption.

*Developed with the goal of turning raw supply chain variables into strategic corporate profit.*
