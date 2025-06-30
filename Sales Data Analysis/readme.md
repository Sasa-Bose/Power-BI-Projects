# 📊 Power BI Project: Sales Data Analysis

This Power BI project presents a comprehensive analysis of sales data using interactive dashboards and advanced data modeling. The objective is to uncover actionable insights such as top-performing products, sales trends, and performance comparisons between different time periods.

---

## 📁 Project Overview

This report includes the following insights and interactive visualizations:

1. **Top/Bottom 5 Products** by:
   - Sales
   - Profit
   - Quantity Sold

2. **Sales Trends** over time:
   - Daily
   - Monthly
   - Quarterly
   - Yearly

3. **Relationship Analysis** between:
   - Sales and Profit

4. **Comparative Analysis**:
   - Compare Sales, Profit, and Quantity Sold between any two user-selected periods

5. **Average Discount** offered in each discount category

6. **Total Number of Orders**

7. **Order-Level Report**:
   - View Sales, Profit, Discount, Net Sales, and more
   - Filterable by Product, Date, Customer ID, and Promotion Category

8. **City-wise Sales Breakdown**

---

## 🛠️ Data Preparation & Modeling Steps

The following steps were performed in Power BI to clean and model the data effectively:

### 🔍 Data Cleaning & Profiling

- Reviewed column data types and profiles in **Power Query Editor**
- Renamed columns to meaningful, consistent names
- Ensured primary keys like `Customer ID` were set to `Text` type
- Cleaned and standardized categorical values (e.g., gender: `M`, `Male`, `1` ➝ `Male`)
- Removed duplicates, handled nulls, and created conditional columns as needed

### 🔗 Data Modeling

- Merged relevant tables
- Added calculated columns (e.g., Profit = 10% of Net Sales)
- Created an **Index column** renamed to `Order ID` for tracking orders

---

## 📊 Key Visualizations

### ✅ Top/Bottom 5 Products

- Bar charts to display Top/Bottom 5 by **Sales**, **Profit**, and **Quantity Sold**
- Created a new `Profit` column in the Fact Table using: Profit = 0.1 * [Net Sales]
  
### 📈 Sales Trend Over Time

- Line chart with drill-through enabled to analyze performance over:
- Daily
- Monthly
- Quarterly
- Yearly timeframes

### 🔄 Comparative Analysis Between Periods

#### Approach 1: Dual Date Tables + DAX

- Created two `Date Tables`: `DateTable1` and `DateTable2` using:
```DAX
DateTable = CALENDARAUTO()
Connected: DateTable1 to Fact Table with Active Relationship
DateTable2 with Inactive Relationship

Created a measure using USERELATIONSHIP:
Sum of Net Sales = CALCULATE(
  SUM('FactTable'[Net Sales]),
  ALL('DateTable1'),
  USERELATIONSHIP('DateTable2'[Date], 'FactTable'[Date])
)
#### Approach 2(Recommended): Visual Interaction Editing
Created two slicers and two sets of charts (Sales, Profit, Quantity)
Used "Edit Interactions" to isolate interactions for each slicer
Reduces model size and improves performance

####📋 Order Table Report with Filters
Table visual displays complete order-level data
Added slicers for: Product, Customer, Date, Promotion
Implemented cross-filtering using this measure: SUM DIM_Filter = SUM('FactTable'[Net Sales])
Applied visual-level filters: Show items where measure is not blank (for dynamic slicer filtering)

###📍 Additional Notes
All custom measures are stored in a separate Measure Table for clarity

###📌 Conclusion
This Power BI project showcases how businesses can use data-driven dashboards to explore sales trends, identify high-performing products, and make informed decisions. The use of calculated measures, dual date tables, and interaction-based filtering demonstrates strong capabilities in handling complex BI requirements.

