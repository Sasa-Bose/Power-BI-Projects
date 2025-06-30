# 🚗 Car Sales Performance Dashboard – Power BI Project

This Power BI dashboard provides a dynamic analysis of car sales across regions, models, and time periods. It features KPIs, trends, and detailed grids to help dealerships and analysts track business performance using powerful time intelligence.

---

## 📸 Dashboard Previews

### 🔹 Overview Page

![Overview Dashboard](./Car%20Sales%20Overview.png)

### 🔹 Details Page

![Details Dashboard](./Car%20Sales%20Details.png)

> Both dashboards are interactive and designed with slicers and filters to support dynamic data exploration.

---

## 📌 Business Objective

To design an end-to-end sales analysis tool for a car dealership network, with an emphasis on:
- Year-over-Year growth and comparisons
- Body style and color distribution
- Regional performance tracking
- Dealer and model-specific insights
- Exportable sales records

---

## 🧠 Project Workflow

1. **Business Requirement Drafting**
2. **Data Import and Validation**
   - Verified **Date** and **Price** fields for completeness and correctness.
   - Used Power Query's **Column Quality/Profile** features.
3. **Data Modeling**
   - Created a **Date table** to support advanced DAX time intelligence.
   - Defined relationships between dimension and fact tables.
4. **DAX Measures**
   - KPIs like `YTD Sales`, `MTD Sales`, `YOY Growth`, and deltas.
5. **Dashboard Layout**
   - Two separate pages: **Overview** (KPI-focused) and **Details** (data table).
   - Slicers for filtering by body style, dealer name, transmission, engine type, etc.

---

## 📊 Key Metrics & Charts

### 🔹 Overview Metrics

| KPI                   | Value     | Insights                    |
|-----------------------|-----------|-----------------------------|
| YTD Total Sales       | $371.2M   | +$70.8M (↑23.6%) YOY        |
| MTD Total Sales       | $54.28M   |                             |
| YTD Avg Price         | $28.0K    | -$0.22K (↓0.79%) YOY        |
| MTD Avg Price         | $28.26K   |                             |
| YTD Cars Sold         | 13.3K     | +2.62K (↑19.73%) YOY        |
| MTD Cars Sold         | 1.92K     |                             |

### 🔹 Visuals on Overview Page

- **Line Chart** – Weekly YTD Sales Trend  
- **Pie Charts** – Sales distribution by Body Style & Color  
- **Map Visual** – YTD Cars Sold by Dealer Region  
- **Company Grid** – Avg Price, Cars Sold, Total Sales, and %GT Sales by Brand  

### 🔹 Details Page (Exportable Grid)

| Column Examples     | Description                             |
|---------------------|-----------------------------------------|
| Car ID              | Unique vehicle identifier               |
| Date                | Sale transaction date                   |
| Customer Name       | Buyer information                       |
| Dealer Name         | Sales point/dealership                  |
| Company / Model     | Brand and model of the car              |
| Color / Body Style  | Aesthetic and vehicle type              |
| Total Sales         | Price paid for the transaction          |

---

## ⚙️ Tools & Techniques

- **Power BI Desktop**
- **Power Query Editor**
- **Custom Date Table**
- **DAX Measures with Time Intelligence**
- **Advanced Slicers**
- **Export-ready Grid View**
- **Map Visuals with Bing Integration**

---

## 📁 Repository Contents

- `Car_Sales_Dashboard.pbix` – Full Power BI report  
- `/screenshots/car_sales_dashboard_overview.png` – Overview Dashboard  
- `/screenshots/car_sales_dashboard_details.png` – Details Table View  
- `README.md` – This documentation  

---

## 📝 Notes

- Ensured all sales records had valid dates and prices (no nulls).
- Optimized for both **executive overview** and **analyst-level drill-down**.
- Grid table can be exported directly by users after applying filters.

---

## ⚠️ Disclaimer

This dashboard uses mock/sample data for demo and educational purposes. It is not affiliated with any real dealerships or automotive companies.

---

## 🔗 Author

**Your Name**  
[LinkedIn](https://www.linkedin.com/in/your-profile) | [GitHub](https://github.com/yourusername)

---
