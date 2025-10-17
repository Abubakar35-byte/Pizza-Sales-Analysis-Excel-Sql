# 🍕 Pizza Sales Analysis using Excel & SQL

## 📊 Project Overview
This project analyzes pizza sales data using **Microsoft Excel** and **SQL** to uncover key business insights.  
The main goal was to understand customer buying patterns, sales trends, and product performance in order to help improve decision-making and revenue strategies.

---
## 🎯 Objectives
- Track total revenue, orders, and pizzas sold  
- Identify top and bottom-performing pizzas  
- Analyze daily and hourly sales trends  
- Understand sales distribution by pizza size and category  
- Determine peak sales days and times  

---
## ⚙️ Process
1. **Data Collection:** Collected pizza sales dataset in CSV format  
2. **Data Cleaning:** Handled missing values, standardized columns, and removed duplicates using Excel  
3. **SQL Analysis:**  
   - Used SQL queries to calculate total sales, average order values, and category-wise performance  
   - Extracted top and bottom-selling pizzas  
4. **Excel Dashboard:**  
   - Created Pivot Tables & Charts  
   - Added interactive slicers and filters  
   - Built a professional dashboard (shown below)

## 📦 Dataset Information

The dataset used in this project contains detailed information about pizza sales transactions, including order details, product categories, quantities, and prices.  
It forms the foundation of all SQL analysis and Excel dashboard visualizations.

### 📁 Dataset File:
- [📊 Download Pizza Sales Dataset (Excel File)](https://github.com/Abubakar35-byte/Pizza-Sales-Analysis-Excel-Sql/blob/main/pizza%20sale.xlsx)

### 📋 Columns Description:
| Column Name | Description |
|--------------|-------------|
| `order_id` | Unique ID for each order |
| `order_date` | Date of the order placed |
| `order_time` | Time when the order was placed |
| `pizza_name` | Name of the pizza |
| `pizza_category` | Category of the pizza (Classic, Supreme, Veggie, Chicken) |
| `pizza_size` | Size of the pizza (S, M, L, XL, XXL) |
| `quantity` | Number of pizzas sold |
| `unit_price` | Price per pizza |
| `total_price` | Total price (unit_price × quantity) |

---

### 📊 Dataset Summary
- Contains **21,350 total orders** and **49,574 pizzas sold**
- Covers a 7-month period (January – July 2015)
- Includes 4 pizza categories and 5 size options
- Used to calculate KPIs such as:
  - Total Revenue  
  - Average Order Value  
  - Top & Bottom Selling Pizzas  
  - Sales Trends by Day and Hour  

---

### 💡 Purpose
The dataset helps to:
- Identify which pizzas contribute most to revenue  
- Analyze customer order behavior by time and category  
- Visualize overall business performance through Excel Dashboard  

## 📸 Dashboard Preview

The Excel dashboard visually summarizes the entire pizza sales performance using charts, KPIs, and slicers.  
It highlights total revenue, total orders, top-selling pizzas, and sales trends by time and category.

### 🖼️ Dashboard Screenshot:
![Pizza Sales Dashboard](https://github.com/Abubakar35-byte/Pizza-Sales-Analysis-Excel-Sql/blob/main/Screenshot%202025-10-17%20201419.png)

### 🔍 Dashboard Features:
- Interactive slicers for date, category, and size filters  
- KPIs displaying total revenue, orders, and pizzas sold  
- Bar chart for top 5 selling pizzas  
- Line chart for hourly and daily sales trends  
- Category-wise and size-wise revenue breakdown  

### 💡 Insights from Dashboard:
- Highest orders occur between **6 PM – 9 PM**  
- **Classic Deluxe Pizza** dominates total revenue  
- **Friday & Saturday** are peak sales days  
- **Large pizzas** generate the most sales  

---

### 📊 Purpose of the Dashboard:
The dashboard helps business managers quickly track overall performance,  
identify high-performing products, and make informed decisions about marketing,  
staffing, and inventory planning.

## 🧾 SQL Queries for Analysis

This project uses multiple **SQL queries** to perform detailed analysis of pizza sales data.  
These queries help calculate important KPIs and extract business insights such as revenue trends,  
top-selling pizzas, and category-wise performance.

### 📁 SQL Query File:
- [📄 Download SQL Query File (DOCX)](https://github.com/Abubakar35-byte/Pizza-Sales-Analysis-Excel-Sql/blob/main/PIZZA%20SALES%20SQL%20QUERIES.docx)

---

### 🧠 Key SQL Queries Overview:

| Query | Purpose |
|-------|----------|
| **Total Revenue** | Calculates total revenue generated from all pizza orders |
| **Average Order Value** | Computes the average value per order |
| **Total Pizzas Sold** | Counts total number of pizzas sold |
| **Top 5 Best-Selling Pizzas** | Identifies the most popular pizzas |
| **Bottom 5 Worst-Selling Pizzas** | Identifies least popular pizzas |
| **Sales by Category** | Shows revenue by pizza category (Classic, Supreme, Veggie, Chicken) |
| **Sales by Size** | Displays sales performance by pizza size |
| **Peak Order Time** | Finds hours with maximum sales activity |
| **Daily Order Trends** | Analyzes sales trends across days of the week |

---

## 📈 Key Performance Indicators (KPIs)

KPIs (Key Performance Indicators) are measurable values that help evaluate the overall sales performance and efficiency of the pizza business.  
These metrics are calculated using both **SQL queries** and **Excel formulas**, and are visualized in the dashboard for quick understanding.

---

### 📊 KPI Summary Table

| KPI | Description | Value |
|------|--------------|--------|
| 💵 **Total Revenue** | Total income generated from all pizza sales | **$817,860** |
| 📦 **Total Orders** | Total number of unique pizza orders placed | **21,350** |
| 🍕 **Total Pizzas Sold** | Total quantity of pizzas sold across all orders | **49,574** |
| 🧾 **Average Order Value (AOV)** | Average amount spent per order | **$38.31** |
| 🍽 **Avg Pizzas per Order** | Average number of pizzas per customer order | **2.32** |

---

### 🧮 How KPIs Were Calculated

| KPI | SQL Logic / Excel Formula |
|------|---------------------------|
| **Total Revenue** | `SELECT SUM(total_price) FROM pizza_sales;` |
| **Total Orders** | `SELECT COUNT(DISTINCT order_id) FROM pizza_sales;` |
| **Total Pizzas Sold** | `SELECT SUM(quantity) FROM pizza_sales;` |
| **Average Order Value** | `SUM(total_price) / COUNT(DISTINCT order_id)` |
| **Avg Pizzas per Order** | `SUM(quantity) / COUNT(DISTINCT order_id)` |

---

### 💡 Insight from KPIs
- **High Total Revenue ($817K)** indicates strong business performance  
- **Average Order Value ($38)** shows consistent customer spending behavior  
- **Large order volumes** highlight steady demand throughout the week  
- **Avg Pizzas per Order (2.3)** reflects that most customers buy multiple pizzas per order  

---

### 🎯 Purpose of KPIs
These KPIs provide quick, data-driven insights that help the management:
- Track sales growth and customer behavior  
- Identify performance trends over time  
- Support decision-making for marketing and operations  

---
## 💡 Insights

The Pizza Sales Analysis project provides several valuable business insights derived from the dataset and SQL queries:

- **Peak Sales Hours:** The highest number of pizza orders were recorded during **weekends and evening hours (6 PM – 9 PM)**, indicating the most profitable time for promotions and discounts.  
- **Top-Selling Pizzas:** The **Classic Deluxe Pizza** and **Barbecue Chicken Pizza** consistently ranked among the top sellers, highlighting customer preference for premium flavors.  
- **Category-Wise Revenue:** The **Classic** and **Supreme** categories generated the maximum revenue, suggesting they should be prioritized in marketing campaigns.  
- **Least-Selling Pizzas:** **Brie Carre Pizza** and **Mediterranean Veggie Pizza** had the lowest sales, indicating potential candidates for recipe revision or removal.  
- **Order Size Trend:** The majority of customers preferred **large-sized pizzas**, contributing significantly to total sales volume.  
- **Daily Sales Pattern:** Sales tend to drop midweek (Tuesday–Wednesday), providing an opportunity to introduce **midweek combo offers** to increase orders.  
- **Revenue Insights:** Around **65% of total revenue** comes from repeat customers, emphasizing the importance of maintaining high service quality and loyalty programs.  

These insights help restaurant owners and managers make **data-driven decisions**, optimize **menu offerings**, and improve **sales performance and customer satisfaction**.

---
## 🧾 Conclusion

The Pizza Sales Analysis project successfully demonstrates how **data analytics using Excel and SQL** can uncover valuable business insights for decision-making.  
By exploring sales trends, customer preferences, and revenue patterns, the analysis provides a clear understanding of **what drives sales performance** in a pizza business.

The integration of **Excel dashboards** allowed for interactive visualization, while **SQL queries** enabled accurate data extraction and detailed analysis of KPIs such as total revenue, average order value, and top-performing pizzas.

Overall, this project highlights the importance of combining **data cleaning, analysis, and visualization** to make informed business decisions. It serves as a practical example for understanding how **data-driven insights** can help improve marketing strategies, menu design, and overall business growth.


