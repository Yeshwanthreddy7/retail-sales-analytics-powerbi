# 📊 Retail Sales Analytics Dashboard (Power BI)

> A professionally designed Power BI dashboard simulating a real-world retail analytics environment with executive-level reporting and interactive insights.

---

## 📌 Project Overview

This project analyzes retail / e-commerce sales data using **Power BI** to generate actionable business insights and performance tracking dashboards.

The goal is to simulate a real-world scenario where management needs to monitor:

- Revenue & Profitability
- Monthly Sales Trends
- Product Performance
- Regional Distribution
- Return Rates & Operational Efficiency

This project focuses on both **business intelligence** and **professional data modeling practices**.

---

## 🎯 Business Objectives

The dashboard answers the following key business questions:

- What is the total revenue, cost, and profit?
- How is revenue trending month-over-month?
- Which products generate the highest revenue?
- Which categories are most profitable?
- How does performance vary by region?
- What is the return rate and its business impact?

---

## 🛠 Tools & Technologies Used

| Tool | Purpose |
|------|---------|
| Power BI Desktop | Dashboard development |
| Power Query | Data cleaning & transformation |
| DAX | Measure creation & KPIs |
| Star Schema Modeling | Professional data modeling |
| Git & GitHub | Version control & project hosting |

---

## 🧠 Data Modeling Architecture

This project follows **industry-standard modeling principles**:

- Fact Table → `Fact_Sales`
- Dimension Table → `DateTable`
- One-to-Many Relationship (Star Schema)
- Time Intelligence enabled via Date Dimension
- Month sorting using `MonthNumber`
- Measures created using optimized DAX

### ✅ Why Star Schema?

- Scalable model
- Accurate aggregations
- Clean separation of facts and dimensions
- Professional BI architecture

---

## 📊 Dashboard Features

### 🔹 Executive KPI Section
- Total Revenue
- Total Cost
- Total Profit
- Total Returns
- Return Rate (%)

---

### 🔹 Sales Trend Analysis
- Monthly Revenue Line Chart
- Time-based performance tracking

---

### 🔹 Product Performance
- Revenue by Product
- Comparative product contribution analysis

---

### 🔹 Category Analysis
- Profit by Category
- Category-level margin visibility

---

### 🔹 Regional Insights
- Interactive Map Visualization
- Region-wise revenue distribution

---

### 🔹 Interactivity
- Region Slicer
- Category Slicer
- Date Range Slicer (Between type)
- Fully dynamic cross-filtering

---

## 🏗 Dashboard Layout Structure

LEFT PANEL → Interactive Filters
TOP ROW → KPI Summary Cards
MIDDLE ROW → Revenue Trend & Product Analysis
BOTTOM ROW → Category Profit & Regional Map


This structure ensures:

- Clear hierarchy
- Executive readability
- Clean UI/UX alignment
- Professional presentation

---

📁 Project Structure
retail-sales-analytics-powerbi/ │ ├── data/ │ └── retail_sales_raw.csv │ ├── pbix/ │ └── retail_dashboard.pbix │ ├── screenshots/ │ └── dashboard.png │ └── README.md


## 📈 Core DAX Measures (Examples)

```DAX
Total Revenue = SUM(Fact_Sales[Revenue])

Total Profit = SUM(Fact_Sales[Profit])

Return Rate = 
DIVIDE(
    SUM(Fact_Sales[Returns]),
    SUM(Fact_Sales[Quantity])
)


## Author

Yeshwanth Reddy
B.Tech – Computer Science & Engineering
Aspiring Data Analytics & UI/UX Professional