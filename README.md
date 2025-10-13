# Sales-and-Product-Analysis-Power-BI-Dashboard

# 🛍️ Online Retail Dashboard – Power BI Project

I’m excited to share my latest analytics project: an **Interactive Online Retail Dashboard** built in **Power BI**, comparing retail performance across **2022–2023** and **2023–2024**.

This project uncovers how customer behaviour, regional performance, and product sales evolved over time — transforming raw sales transactions into clear business insights.

---

## 📈 What the Data Reveals

### 💰 **1. Sales Momentum**
- Total sales reached **£29.04M**, driven by a 16M-unit volume across two years.  
- A strong **104% year-on-year sales growth** signals a solid recovery and expansion.  
- The final quarter of 2023–2024 outperformed the previous year by more than **90%**, highlighting end-of-year demand peaks.

---

### 🧩 **2. Product Insights**
- The **top five products** generated over **40% of total sales**, indicating high product concentration.  
- Average Order Value rose from **£541.42**, supported by cross-selling and multi-item orders.  
- Certain SKUs saw rapid YoY growth, while a few mature products declined — clear signals of evolving consumer preferences.

---

### 🌍 **3. Regional Breakdown**
- **Switzerland, Spain, and Sweden** led in sales, contributing more than 80% of total units sold.  
- Smaller markets such as **Singapore and Thailand** show room for expansion.  
- Seasonal demand spikes are visible across most regions, mirroring global retail cycles.

---

### 👥 **4. Customer Behaviour**
- Over **5,900 unique customers** were analysed.  
- Returning customers consistently placed higher-value orders, while new customers showed lower frequency but strong engagement potential.

---

## 📊 Dashboard Pages

| Page | Focus | Highlights |
|------|--------|-------------|
| **Summary Page** | Executive overview | KPIs, quarterly trend, top countries, product mix |
| **Sales Analytics Page** | Regional and temporal trends | Year-on-year growth, monthly trends, regional contribution |
| **Product Analysis Page** | Product-level insights | Sales growth contribution, AOV trends, country distribution |

---

## 🧮 Key Technical Approach

- **Data Source:** [Online Retail II Dataset (UCI Machine Learning Repository)](https://archive.ics.uci.edu/ml/datasets/Online+Retail+II)  
- **Data Cleaning:** Power Query – removed null CustomerIDs, handled duplicates, merged two yearly tables.  
- **Data Modelling:**  
  - Star schema with **Fact_Transactions** and **Dimension tables** (Date, Product, Country, Customer).  
- **Core DAX Measures:**  
  - `Total Sales = SUMX(Fact_Transactions, Quantity * Price)`  
  - `Sales Growth % = DIVIDE([Sales 2023-24] - [Sales 2022-23], [Sales 2022-23])`  
  - `AOV = DIVIDE([Total Sales], DISTINCTCOUNT(Invoice))`  
- **Analytics Techniques:**  
  - Year-on-Year (YoY) comparison  
  - Growth contribution analysis  
  - KPI variance indicators  
  - Dynamic page navigation with bookmarks and buttons  
  - Searchable slicers for interactive filtering  

---

## 📷 Dashboard Preview

### 🧭 **Summary Page**
![Summary Page](Screenshots/Summary%20Page.png)

---

### 📈 **Sales Analytics Page**
![Sales Analytics Page](Screenshots/Sales%20Analytics%20Page.png)

---

### 📦 **Product Analysis Page**
![Product Analysis Page](Screenshots/Product%20Analysis%20Page.png)

---

## 💡 Key Insights at a Glance
| Metric | 2022-2023 | 2023-2024 | Growth |
|---------|------------|------------|---------|
| Total Sales (£) | £9.5M | £19.5M | **+104%** |
| Units Sold | 8M | 8M | — |
| Average Order Value | £270 | £541 | **+100%** |
| Distinct Products | 2,500 | 5,100 | **+104%** |

---

## 🎯 Takeaway
The dashboard highlights how a business can leverage Power BI to monitor year-on-year performance, pinpoint growth drivers, and visualise where value is being created — across both **products** and **regions**.  

A clear example of turning raw transactional data into meaningful, visual stories that drive business decisions.
⭐ *If you found this analysis insightful, feel free to star the repository and explore my other projects like the [Netflix Dashboard](https://github.com/NeerajRaj796/Netflix_Dashboard.git).*
