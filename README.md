📊 Sales Dashboard (Power BI)

This is my first Power BI project, where I created a simple sales dashboard to explore and analyze sales data.

The dataset includes product sales details such as order date, sales amount, sales quantity, and customer information.
I used Power BI to clean the data, perform transformations, and build a dashboard for visualization.

🔧 What I Did

Cleaned and transformed raw sales data in Power Query

Created a new calculated column for Cost Price,Normalized Sales Amount etc

Built a dashboard to visualize sales insights

Gained hands-on experience in Power BI basics

🛠 Tools Used

Power BI Desktop
MySQL Workbench
Power Query

Data Analysis Using SQL Query=>
Show all customer records
SELECT * FROM customers;
Show total number of customers
SELECT count(*) FROM customers;
Show transactions for Chennai market (market code for chennai is Mark001
SELECT * FROM transactions where market_code='Mark001';
Show distrinct product codes that were sold in chennai
SELECT distinct product_code FROM transactions where market_code='Mark001';
Show transactions where currency is US dollars
SELECT * from transactions where currency="USD"
Show transactions in 2020 join by date table
SELECT transactions.*, date.* FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020;
Show total revenue in year 2020,
SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.currency="INR\r" or transactions.currency="USD\r";
Show total revenue in year 2020, January Month,
SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and and date.month_name="January" and (transactions.currency="INR\r" or transactions.currency="USD\r");
Show total revenue in year 2020 in Chennai
//SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.market_code="Mark001";
Output:
<img width="1154" height="732" alt="image" src="https://github.com/user-attachments/assets/d5a342e9-9132-4025-8053-8c3ac44d1095" />
