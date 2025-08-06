
# 🧾 Apocalypse Store Sales Dashboard

An interactive Power BI dashboard visualizing retail sales data for Apocalypse Store. Designed to provide clear, actionable insights into revenue, profit, product performance, and regional trends.

---

## 📌 Project Overview

This dashboard delivers a comprehensive overview of Apocalypse Store's sales performance. It uses DAX-powered KPIs, filters, and visuals to help stakeholders track trends, spot top-performing products, and assess business health over time.

---

## 📁 Datasets

- **Sales Table**
  - Fields: Order ID, Date, Product ID, Quantity Sold, Revenue, Profit
- **Products Table**
  - Fields: Product Name, Category, Subcategory, Price, Cost
- **Region Table**
  - Fields: Store Name, Region, Location

---

## 📐 Measures (DAX)

- `Total Revenue = SUM(Sales[Revenue])`
- `Total Profit = SUM(Sales[Profit])`
- `Total Orders = DISTINCTCOUNT(Sales[Order ID])`
- `Profit Margin = DIVIDE([Total Profit], [Total Revenue])`
- `Monthly Sales = CALCULATE([Total Revenue], DATESMTD(Sales[Date]))`
- `Top Products Rank = RANKX(ALL(Products[Product Name]), [Total Revenue])`

---

## 📊 Visuals & Insights

- **KPI Cards**
  - 💰 Total Revenue
  - 📦 Total Orders
  - 📈 Profit
  - 🧮 Profit Margin

- **Line Chart**
  - Sales trends by month/year

- **Bar Chart**
  - Top 10 best-selling products

- **Donut Chart**
  - Sales by region

- **Clustered Bar**
  - Profit by product category

---

## 🎯 Key Insights

- Top-performing product categories contribute disproportionately to total revenue.
- Revenue spikes during specific months—potential promotional or seasonal campaigns.
- Region-wise performance highlights high and low-performing territories.
- Profit margin trends help assess cost management efficiency.

---

## 🎛️ Filters Available

- Date Range (Calendar slicer)
- Product Category
- Region
- Product Name

---

## 📷 Screenshots

### 📌 Overview Dashboard  
![Dashboard Overview](35840b3c-6170-4c1a-ace4-d692cb66797e.png)

### 💼 Profit by Customer  
![Profit by Customer](b86d5c07-1702-4b35-a5af-945fedfa481c.png)  
> *Displays total profit contribution by each customer.*

---

## 🚀 How to Use

1. Download the `.pbix` file (Power BI Desktop required).
2. Open in Power BI Desktop.
3. Use the filters to explore trends across categories, regions, and time.
4. Export insights as reports for stakeholders.

---

## 📬 Contact

Created by **Obed3690**  
🌍 GitHub: [github.com/Obed3690](https://github.com/Obed3690)

---

## 📄 License

MIT License – free to use, modify, and distribute.
