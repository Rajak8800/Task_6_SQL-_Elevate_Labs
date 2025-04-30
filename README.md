# Task_6_SQL-_Elevate_Labs

# 🧠 SQL Business Analysis – Task 6 (Elevate Labs)

This project contains SQL queries and insights developed to analyze sales and return data using MySQL. The dataset includes information on orders, returns, customers, and products.

## 📂 Project Structure

- `Task_6_Elevate_Labs_SQL.sql` – SQL file with all queries, joins, and analysis
- `SQL_Analysis_Report.docx` – Professional report (optional Word format)
- `README.md` – This file

## 📊 Key Business Questions Answered

1. Monthly Sales Trend
2. Monthly Return Rate
3. Sales by City
4. Total Orders & Returns
5. Profit by Region
6. Average Shipping Time
7. Top Categories by Quantity Sold
8. Highest Sales by Product
9. Monthly Profit Trend
10. Category-wise Return Rate

Each question includes:
- ✅ SQL query
- 📈 Output
- 💡 Business Insight

## 🛠️ Tools Used

- **SQL** – MySQL 8+
- **MySQL Workbench** or any SQL editor
- **Power BI / Word** – Optional visualization or reporting

## 🧾 Sample Query

```sql
SELECT 
    DATE_FORMAT(order_date, '%b') AS Month, 
    ROUND(SUM(sales), 2) AS Total_Sales
FROM Orders_data
GROUP BY MONTH(order_date)
ORDER BY MONTH(order_date);
