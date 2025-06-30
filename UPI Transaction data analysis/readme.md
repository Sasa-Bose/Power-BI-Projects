# 💳 Power BI Project: UPI Transaction Data Analysis

This Power BI report provides an in-depth analysis of Unified Payments Interface (UPI) transaction data in India. The dashboard is designed to be highly interactive and user-friendly, helping users understand key metrics like transaction volumes, balances, and trends across various dimensions like city, currency, app, and time.

---

## 📁 Project Overview

The report delivers insights on:

1. **Total Transactions** and **Transaction Value** trends
2. **UPI App-wise** performance analysis
3. **Bank-wise** transaction breakdown
4. **State and City-level** adoption metrics
5. **Monthly and Quarterly growth patterns**
6. **Transaction Count vs. Value comparisons**
7. **Remaining Balance vs. Transaction Amount**
8. **Currency-level transaction tracking**

---

## 🧠 Key Features & Techniques

### 🔄 Synced Slicers Across Pages

- 10 well-structured slicers (5 per row) for:
  - State
  - UPI App
  - Bank
  - Date
  - Transaction Type
- Manually sized and aligned for consistent layout
- Synced across all report pages for seamless filtering

### 🎨 Conditional Formatting

- Color scales used to highlight:
  - High/low transaction volumes
  - Exceptional balance trends
- Applied to:
  - Matrix

### 🔖 Bookmarks with Interactive Buttons

A dynamic chart-switching system using bookmarks and buttons:

- **4 toggle buttons**:
  - Line Chart – Transaction Amount
  - Column Chart – Transaction Amount
  - Line Chart – Balance Inquiries
  - Column Chart – Balance Inquiries
- Users can click buttons to instantly switch chart types
- Bookmarks linked with Selection Pane to show/hide visuals accordingly

### 📊 Matrix Visual (Special Use Case)

- A **matrix** was created to display:
  - **Transaction Amount** and **Remaining Balance**
  - Across **months of 2024**
  - For **different cities**
- Provides a multi-dimensional view of performance
- Enhanced with conditional formatting for quick pattern recognition

---

## 📊 Visuals Used

- Line and Column Charts (toggleable via bookmarks)
- Matrix Visuals
- Slicer Grid with Syncing

---

## 🛠️ Data Preparation Highlights

- Cleaned and standardized:
  - App Names
  - State, City, Bank Names
  - Currency Formats
- Used calculated columns for:
  - Year, Month, Quarter
- Created DAX measures for:
  - Total Transaction Amount
  - Balance Inquiries
  - Remaining Balance
  - Average Value per Transaction

---

---

## ✅ User Experience Enhancements

- 🎛️ **Slicer syncing** across pages for consistent filtering
- 🎨 **Conditional formatting** to make outliers pop
- 🔘 **Bookmarks and toggle buttons** for real-time chart switching
- 📊 **Matrix visual** to break down metrics by city, currency, and month
- 📐 Carefully designed layout for readability and user control

---

## 📌 Conclusion

This UPI Transaction Analysis dashboard offers a comprehensive and dynamic way to explore India's digital payment ecosystem. It goes beyond standard reporting by implementing slicer syncing, conditional formatting, visual bookmarks, and matrix views — ensuring both analytical depth and a high-quality user experience.

---
