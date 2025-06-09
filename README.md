☕ Coffee Shop Sales Analysis Dashboard
======================================

📊 Overview
-----------
This project delivers an insightful data analysis and interactive visualization of a fictional coffee shop’s sales data. Utilizing PostgreSQL for querying and Power BI for dashboarding, it uncovers key trends in sales performance, customer behavior, and product preferences, helping stakeholders make data-driven decisions.

🔍 Objective
------------
Analyze sales transactions across time, store locations, and product categories to reveal actionable insights that improve store efficiency and enhance product offerings.

🧰 Tools & Technologies
-----------------------
-  Database: PostgreSQL
-  Data Visualization: Power BI
-  Query Language: SQL
-  Dataset: Coffee Shop Sales Data (.csv)

📌 Key Features
---------------
- Interactive Dashboard showcasing KPIs: Total Sales, Orders, and Quantity Sold
- Time-based analyses: Monthly growth, daily trends, peak sales hours
- Performance comparison across store locations
- Product category and product type trend insights

🧾 SQL Analysis Highlights
--------------------------
📏 Key Performance Indicators (KPIs):
💰 Total Sales
🛒 Total Orders
📦 Total Quantity Sold

📈 Trend Analyses:
- Month-over-Month (MoM) Growth
- Weekday vs Weekend Sales Patterns
- Peak Hour Sales Analysis
- Top 10 Product Types by Sales
- Store Location Performance

📝 Sample SQL Query: Sales by Location for June
-----------------------------------------------
SELECT store_location, 
       ROUND(SUM(unit_price * transaction_qty) / 1000, 1) || ' K' AS total_sales
FROM coffee_shop_sales
WHERE EXTRACT(MONTH FROM transaction_date) = 6
GROUP BY store_location
ORDER BY total_sales DESC;

📈 Dashboard Preview
--------------------
(*Add screenshots or link to Power BI dashboard here*)

🚀 How to Use
-------------
1. Clone this repository
2. Load the dataset into your PostgreSQL database
3. Run the SQL queries to generate insights
4. Open the Power BI `.pbix` file
5. Connect Power BI to your PostgreSQL database (if applicable)
6. Explore the interactive dashboard and visualizations

📂 Repository Structure
-----------------------
Coffee_Shop_Analysis/
  ├── Coffee_shop.pbix                # Power BI Dashboard file
  ├── SQL_Queries_Coffee_Shop.docx   # Document with SQL queries for KPIs and trends
  └── README.txt                     # Project documentation

👤 Author
---------
Mareeswaran A  
Aspiring Business Analyst | Data Enthusiast  
🔗 LinkedIn: https://www.linkedin.com/in/mareeswarana  
✉️ Email: mareeswarana465@gmail.com
