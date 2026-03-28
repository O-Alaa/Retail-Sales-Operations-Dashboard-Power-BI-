# 📊 Super Store Sales & Operations Analysis (Power BI)

## 📌 Project Overview

This project is a complete Business Intelligence dashboard built using **Power BI** to analyze Super Store sales data and generate actionable business insights.

The dashboard focuses on:

- Sales Performance
- Customer Insights
- Product Category Analysis
- Shipping & Operational Efficiency

This project demonstrates skills in:
- Data Cleaning
- Data Modeling
- DAX Calculations
- KPI Design
- Business Storytelling

---

# 🖥 Dashboard Preview

---

## 1️⃣ Sales Performance Overview

![Dashboard Page 1](/images/proj3_page1.png)

### Key Metrics:
- Total Sales
- Total Orders
- Average Sales per Order
- Average Shipping Days

### Insights Delivered:
- Sales growth trend over time
- Regional performance comparison
- Segment contribution to revenue
- Shipping mode performance impact

---

## 2️⃣ Customer Insights

![Dashboard Page 2](/images/proj3_page3.png)

### Focus:
- Sales Trend by Segment Over Time
- Sales by Region
- Top Customers by Revenue
- Customer Segment Contribution

### Business Value:
Identifies high-value customers and profitable segments.

---

## 3️⃣ Product Category Analysis

![Dashboard Page 3](/images/proj3_page2.png)

### Focus:
- Sales by Category
- Sales by Sub-Category
- Top 10 Products by Sales
- Category Performance Distribution

### Business Value:
Helps identify best-performing product lines and optimization opportunities.

---

## 4️⃣ Shipping & Operations

![Dashboard Page 3](/images/proj3_page4.png)

### Metrics:
- Average Shipping Days
- Orders by Shipping Mode
- Shipping Efficiency Trend

### Business Value:
Evaluates operational performance and delivery efficiency.

---

# 🧠 Data Preparation & Modeling

- Fixed incorrect Order Date formatting issues.
- Created a proper Date hierarchy.
- Created calculated column for Shipping Days:

---
### Shipping Days Calculation

Since the dataset does not provide shipping duration, a calculated column was created to measure operational efficiency:

```DAX
Shipping Days = DATEDIFF('Orders'[Order Date], 'Orders'[Ship Date], DAY)
