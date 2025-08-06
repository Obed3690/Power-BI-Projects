
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
![Dashboard Overview]<img width="1210" height="545" alt="image" src="https://github.com/user-attachments/assets/029cc4aa-23ef-49d3-8eb2-237f6be49e57" />



### 💼 Number of Sales by Customer  
![Number of Sales by Customer]<img width="350" height="182" alt="image" src="https://github.com/user-attachments/assets/f7401d9f-48ab-4915-aeb6-41c5e92c9401" />
  
> *Displays the number of sales made by each customer.*


### 💼 Total Products Sold  
![Total Products Sold]<img width="342" height="201" alt="image" src="https://github.com/user-attachments/assets/1d9c61f6-f93b-4988-82c8-6e404590ce05" />
  
> *Displays total Products sold by the store.*


> ### 💼 Units of Product Sold within the Week  
![Products sold within the days of the week]<img width="681" height="265" alt="image" src="https://github.com/user-attachments/assets/64d655cb-990c-47ff-9757-dfeaf34511bf" />
  
> *Displays and analyzes the number of days the store makes more sales.*

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
