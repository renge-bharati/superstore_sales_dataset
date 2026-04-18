# 📊 Superstore Sales Data Analysis Project

## 📝 Project Overview
This project analyzes a retail sales dataset to extract meaningful insights and support business decision-making using Excel, SQL, and Power BI.

---

## 🎯 Objectives
- Analyze overall sales performance  
- Identify top-performing products and regions  
- Understand monthly sales trends  
- Build an interactive dashboard  

---

## 🛠️ Tools & Technologies
- Microsoft Excel (Data Cleaning)
- SQL (Data Analysis)
- Power BI (Data Visualization)

---

## 📂 Dataset
- Name: Superstore Sales Dataset  
- Type: CSV / Excel  
- Description: Contains order, product, sales, and regional data  

---

## 🔍 Process

### 🔹 Data Cleaning (Excel)
- Removed duplicate records  
- Handled missing values  
- Converted date format  

### 🔹 Data Analysis (SQL)

```sql
-- Total Sales
SELECT SUM(Sales) AS Total_Sales FROM superstore;

-- Sales by Region
SELECT Region, SUM(Sales) AS Total_Sales
FROM superstore
GROUP BY Region
ORDER BY Total_Sales DESC;

-- Monthly Sales Trend
SELECT MONTH(Order_Date) AS Month, SUM(Sales) AS Total_Sales
FROM superstore
GROUP BY Month
ORDER BY Month;
