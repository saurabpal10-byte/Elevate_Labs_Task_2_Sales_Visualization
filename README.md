# Elevate Labs – Task 2: Data Visualization and Storytelling

## 📊 Sales & Profit Performance Dashboard

This project was completed as part of the **Elevate Labs Data Analyst Internship – Task 2: Data Visualization and Storytelling**.

The objective of this task was to create meaningful visualizations that communicate sales and profitability patterns through an interactive Power BI dashboard.

---

## 🎯 Objective

The main objective of this project is to:

- Create effective data visualizations.
- Present sales and profitability performance clearly.
- Identify patterns across categories, regions, customer segments, sub-categories, and time.
- Apply appropriate chart types for different data dimensions.
- Create a business-focused visual story rather than presenting charts without context.
- Summarize the key findings in a dedicated Business Insights page.

---

## 🛠️ Tools Used

- **Power BI Desktop**
- **Microsoft Excel / CSV dataset**
- **GitHub**
- **DAX**

---

## 📂 Dataset

The project uses a **Superstore sales dataset** containing sales-related information such as:

- Order Date
- Order ID
- Customer ID
- Customer Name
- Category
- Sub-Category
- Region
- Segment
- Sales
- Profit
- Quantity
- Product information

The dataset was used to analyze sales and profitability performance across different business dimensions.

---

# 📈 Dashboard Overview

The Power BI dashboard is titled:

**Sales & Profit Performance**

It provides an executive-level overview of sales and profitability.

### Key Performance Indicators

The dashboard contains four KPI cards:

| KPI | Value |
|---|---:|
| Total Sales | 2.33M |
| Total Profit | 292.30K |
| Total Orders | 5K |
| Profit Margin | 12.56% |

---

## 📊 Visualizations

### 1. Sales by Category

A column chart showing total sales across:

- Technology
- Furniture
- Office Supplies

Technology has the highest sales among the three categories.

---

### 2. Monthly Sales & Profit Trend

A line chart showing monthly Sales and Profit trends across the year.

The visualization helps identify changes in sales and profitability throughout the displayed period.

---

### 3. Profit by Sub-Category

A horizontal bar chart showing profit across product sub-categories.

Conditional formatting is used to distinguish profitability:

- 🟢 Green → Positive profit
- 🔴 Red → Negative profit

The chart highlights sub-categories with negative profit, including:

- Supplies
- Bookcases
- Tables

---

### 4. Sales by Region

A column chart comparing sales across:

- West
- East
- Central
- South

The West region has the highest sales among the four regions.

---

### 5. Sales by Customer Segment

A donut chart showing sales contribution from:

- Consumer
- Corporate
- Home Office

The displayed sales contribution is:

- Consumer: **50.32%**
- Corporate: **30.77%**
- Home Office: **18.92%**

---

## 🎛️ Interactive Filters

The dashboard includes interactive filters for:

### Order Date

Users can filter the dashboard by the selected order-date range.

### Region

- Central
- East
- South
- West

### Category

- Furniture
- Office Supplies
- Technology

These filters allow users to explore the dashboard from different perspectives.

---

# 💡 Business Insights

## 1. Category Performance

Technology generates the highest sales among the three product categories, followed by Furniture and Office Supplies.

## 2. Regional Performance

The West region has the highest sales, followed by East, Central, and South.

## 3. Customer Segment

Consumer customers account for approximately **50.3%** of total sales, followed by Corporate at approximately **30.8%** and Home Office at approximately **18.9%**.

## 4. Monthly Trend

Sales fluctuate throughout the year, with noticeably higher sales toward **September and November–December** in the displayed monthly trend.

## 5. Profit Concentration

Copiers, Phones, and Accessories appear among the higher-profit sub-categories in the displayed chart.

These insights are observations from the dashboard visualizations and do not assume the reasons behind the observed patterns.

---

# 📐 DAX Measures

The dashboard uses DAX measures for the main KPIs.

### Total Sales

```DAX
Total Sales = SUM(Orders[Sales])
