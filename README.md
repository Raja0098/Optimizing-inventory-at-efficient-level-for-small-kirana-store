# Optimizing-inventory-at-efficient-level-for-small-kirana-store

This project applies data-driven techniques to optimize inventory levels for a small Kirana (convenience) store in Masaurhi, Patna, Bihar, with the goal of minimizing stockouts and improving capital efficiency. All analysis was performed using Microsoft Excel and google colab on 30 days of manually collected sales data across 49 SKUs.

---
## 🧠 Problem Overview

Ajay Kirana Store, operating since 2005, faced difficulty managing stock levels due to limited capital post-COVID. The owner relied solely on experience for restocking, leading to:

- Frequent stockouts
- Inability to invest in fast-moving/growing SKUs
- Poor working capital management

This project aims to:

✅ Analyze sales patterns  
✅ Forecast future demand  
✅ Define efficient restocking policies  
✅ Determine reorder points and safety stock

---
## 📈 Tools & Technologies

- **Excel and google colab ** (tool for analysis)
- Data cleaning & transformation
- Pivot Tables, Charts, Graphs
- Moving Average Forecasting
- ABC Analysis
- Statistical formulas (Standard Deviation, Z-score, Safety Stock)

---

## 🧪 Analysis Process & Methodology

### 1. 📊 Data Cleaning
- Removed SKUs with zero or negligible sales
- Filled missing values with 0

### 2. 📈 Exploratory Data Analysis (EDA)
- Calculated mean, max, variance, and standard deviation for each SKU
- Built pivot tables to aggregate sales per SKU

### 3. 📉 Pareto Analysis
- Volume Pareto: Identified SKUs with high sales volume
- Revenue Pareto: Identified SKUs contributing most to revenue
- Visualized using bar charts

### 4. 🗃️ Category-wise Aggregation
- Grouped SKUs by categories (e.g. Snacks, Essentials)
- Calculated category-wise monthly sales and revenue
- Plotted bar graphs for better visibility

### 5. 📅 Weekly Trend Analysis
- Aggregated sales weekly (Week 1 to Week 4)
- Analyzed demand spikes across categories by week

### 6. ⏳ Time Series Forecasting
- Applied 5-day moving average to forecast demand
- Plotted trend lines to visualize actual vs. forecasted sales

### 7. 🧠 ABC Analysis
- Categorized SKUs based on importance and sales volume
- Identified high-priority SKUs for inventory focus

### 8. 🧮 Reorder & Safety Stock Strategy
For each SKU:
- **Average Demand**
- **Lead Time** = 1 day (local supplier)
- **Standard Deviation of demand**
- **Service Level**: 99% for Essentials, 95% for others
- **Z-score** using Excel formula `=NORM.S.INV(%)`
- **Safety Stock** = `Z * σ * √LT + Avg Demand * LT`
- **Reorder Point** = `Avg Demand * LT + Safety Stock`

---

## 📊 Project Outputs

- 📌 SKU-level safety stock & reorder points
- 📌 Weekly ordering strategy (vs daily)
- 📌 Focus list of top SKUs (based on revenue & volume)
- 📌 Suggested weekly/monthly restocking windows
- 📌 Opportunities for investing in fast-growing products (e.g., Bisleri bottles)

---
## 📚 Business Impact

✅ Eliminated guesswork in restocking  
✅ Reduced stockouts for essentials  
✅ Enabled data-driven working capital allocation  
✅ Created a scalable, repeatable Excel-based analysis process for other small stores

## 📌 Future Work

- Integrate POS systems for automated data tracking  
- Expand to more SKUs and longer timeframes  
- Automate reporting using Python or Power BI  
- Use ARIMA/Prophet models for advanced forecasting  
- Implement dashboards for real-time decision-making

---

## 🤝 Acknowledgments

Thanks to **Ajay Kirana Store** for their collaboration, openness, and support in sharing business insights and real data for this impactful project.

---

## 📜 License

This project is shared for educational and portfolio purposes.
