# 📊 Power BI Project: Sales Data Analysis

This Power BI project provides a comprehensive sales data analysis dashboard built in Power BI. The dashboard includes detailed insights into product performance, sales trends, discounts, and regional analysis. Interactive filters and dynamic visuals allow users to explore data efficiently and compare performance across time periods.

---

## 📁 Project Overview

The dashboard includes the following key insights:

1. **Top/Bottom 5 Products** by:
   - Sales
   - Profit
   - Quantity Sold

2. **Sales Trends** across:
   - Daily
   - Monthly
   - Quarterly
   - Yearly periods

3. **Sales vs. Profit Relationship**

4. **Compare Metrics** (Sales, Profit, Quantity Sold) between any two user-defined time periods

5. **Average Discount** by Discount Category

6. **Total Number of Orders**

7. **Order-Level Table View**:
   - Fields: Sales, Profit, Discount, Net Sales, etc.
   - Filterable using Product, Date, Customer ID, Promotion Category

8. **Sales by City**

---

## 🛠️ Data Preparation and Modeling Steps

### 🔹 Data Cleaning

- Checked column data types and profiles in Power Query Editor
- Standardized column names and values (e.g. gender formats, binary labels)
- Removed duplicates, nulls, and invalid entries
- Converted identifiers like `Customer ID` and `Order ID` to text
- Created conditional columns where needed

### 🔹 Data Modeling

- Merged tables where appropriate
- Created calculated columns (e.g. Profit = 10% of Net Sales)
- Added Index column renamed to `Order ID`
- Applied single-directional relationships between dimension and fact tables
- Ensured related columns are of the same data type
- Used “Assume Referential Integrity” where possible

---

## 📊 Key Visuals and Techniques

### ✅ Top/Bottom 5 Products

- Used **Stacked Bar Charts**
- Applied **Visual-Level Filters** to show Top/Bottom 5 for Sales, Profit, and Quantity Sold
- Used a **calculated column** to estimate Profit as 10% of Net Sales (based on business rule)

### 📈 Sales Trend Over Time

- Used **Line Charts**
- Enabled **Drill-through** to analyze data by day, month, quarter, and year

### 🔄 Period-to-Period Comparison

#### Method 1: Using Dual Date Tables and DAX Measures

- Created two **Date Tables**
- Defined one **active** and one **inactive** relationship
- Created custom measures using DAX functions such as:
  - `CALCULATE`
  - `USERELATIONSHIP`
  - `ALL`
- Used **Bar Charts** to visualize metric comparisons between selected periods

#### Method 2 (Recommended): Using Interaction Settings

- Added **two date slicers**
- Created **two sets of visuals** (Sales, Profit, Quantity)
- Configured **Edit Interactions** so each set responds to its respective slicer
- Avoided extra date tables for better performance

[Two different date filters for comparing two different periods](./Two%20periods%20compared.png)
---

## 📋 Order-Level Detail (Requirement 7)

- Used **Table Visual**
- Added slicers for:
  - Product Name
  - Customer Name
  - Promotion Name
  - Date
- Enabled **cross-filtering between slicers** using DAX measures and **Visual-Level Filters**
- Used DAX function:
  - `SUM`

---

## 🔢 KPI & Summary Metrics

- Used **Card Visuals** for KPIs:
  - Total Orders (using `DISTINCTCOUNT`)
  - Total Sales, Profit, and Quantity Sold

- Calculated **Average Discount by Category** using bar chart and the `AVERAGE` function

- All measures organized into a dedicated **Measure Table**

---

## 🌍 City-Wise Sales Breakdown

- Used **Bar/Map Visuals** to display sales performance by city
- Enabled filtering and sorting by performance metrics

---

## 📌 Conclusion

This project demonstrates a full-cycle business intelligence solution, showcasing:

- Data cleaning and modeling best practices
- Effective use of DAX for calculated metrics and dynamic filtering
- Advanced filtering techniques using dual slicers and interaction settings
- Interactive and user-friendly dashboards for data exploration

The report enables businesses to identify top-performing products, understand sales patterns, compare across periods, and make informed decisions.

---
