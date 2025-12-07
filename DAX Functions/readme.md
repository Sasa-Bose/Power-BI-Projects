# 📊 Power BI Sales Analytics Report

## 📌 Overview
This project is a comprehensive Power BI analytics solution built on a clean star-schema data model. It provides insights into sales, returns, customers, product performance, and regional trends using interactive multi-page dashboards and a rich library of DAX measures.

---

## 📁 Dataset & Data Model

### **Tables Used**
**Fact Tables**
- `Fact Sales`
- `Fact Returns`

**Dimension Tables**
- `Dim Product Category`
- `Dim Product Subcategory`
- `Dim Products`
- `Dim Customers`
- `Dim Territory`
- `Dim Calendar` (marked as Date Table)

### **Data Model Structure**
- Implemented a **star schema** for efficiency and clarity.
- Fact tables connected to conformed dimensions using surrogate keys.
- Snowflake design for Product Category → Subcategory → Products.
- `Dim Calendar` drives all time intelligence calculations.

---

## 🧮 DAX Measures & KPIs

All measures are organized inside a **Key Measures folder**, grouped into meaningful sub-folders.

### **DAX Concepts Covered**
- **Basic Measures**: SUM, COUNT, AVERAGE  
- **Iterator Functions**: SUMX, AVERAGEX, MINX, MAXX  
- **Filter Functions**: CALCULATE, FILTER, ALL, REMOVEFILTERS, ALLEXCEPT  
- **Logical Functions**: IF, SWITCH, AND/OR, ISBLANK  
- **Math Functions**: DIVIDE, ROUND, VAR calculations  
- **Text Functions**: FORMAT, CONCATENATE, LEFT/RIGHT/MID  
- **Table Functions**: SUMMARIZE, ADDCOLUMNS, CROSSJOIN  
- **Relationship Functions**: USERELATIONSHIP, CROSSFILTER  
- **Ranking & Sorting**: TOPN, RANKX  
- **Running Totals**  
- **Time Intelligence**: YTD, QTD, MTD, PY, YOY%, SAMEPERIODLASTYEAR, DATEADD  

### **Key KPIs**
- Total Sales  
- Total Returns  
- Net Sales  
- Gross Profit & Gross Margin %  
- Return Rate  
- Year-over-Year Sales & Growth %  
- Top/Bottom Products, Customers & Regions  
- Monthly & YTD Trends  

---

## 📄 Report Pages & Visualizations

The Power BI report contains multiple pages showcasing rich, interactive visuals:

- **Executive Summary** – high-level KPIs and trends  
- **Sales Performance** – trends, comparisons, running totals  
- **Product Insights** – category/subcategory/product breakdown  
- **Customer Analysis** – segmentation, rankings, demographics  
- **Territory Overview** – geographic and regional performance  
- **Returns Analysis** – return trends, rates & product impact  
- **Time Intelligence View** – YTD, PY comparisons, seasonality  

Includes slicers, drill-through, bookmarks, and interactive tooltips.

---

## 🧼 Data Preparation & Transformation

Performed in **Power Query**:
- Corrected data types  
- Cleaned and standardized fields  
- Built and marked a dedicated Date table  
- Created product hierarchies  
- Removed duplicates  
- Ensured referential integrity  
- Added calculated columns where necessary  

---


---

## 🛠 Tools & Technologies
- **Power BI Desktop**
- **Power Query (M Language)**
- **DAX (Data Analysis Expressions)**
- **Star Schema Data Modeling**

---

## ▶️ How to Use the Report
1. Open the `.pbix` file in Power BI Desktop.  
2. Refresh data sources if needed.  
3. Navigate using page tabs or navigation buttons.  
4. Use slicers to filter by date, product, customer, and region.  
5. Hover on visuals for tooltips and drill-through options.

---

## 🎯 Project Goals
- Build an optimized, easy-to-maintain Power BI data model  
- Provide accurate KPIs and insights using advanced DAX  
- Enable deep analysis across products, customers, and territories  
- Create intuitive, interactive dashboards for decision-making  

---

## 🗂 Measure Folder Structure
