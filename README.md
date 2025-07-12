# Sales Insight Dashboard using PowerBI


## Problem statement

AtliQ hardware is a company which delivers computer hardware & peripheral 
Manufacturers to his clients, which has several branches throughout India. The sales director of the company is facing a lot of
issues in terms of understanding how the business is performing and what are all the problem company is
facing currently as the sales are not as expected and declining gradually. And whenever he calls the regional managers
to get the current status of the sales and market, as a human behaviour, these people 
Humans are not comfortable in consuming numbers from excel files, which is obvious reason for the frustration.

## Solution

Sales director of the AltiQ hardware, decided to build a PowerBI Dashboard for converting the data into 
visual representation to make data driven decisions. So, he hired a team of data people to complete this task.

## Using Sql Commands 

Show all customer records

SELECT * FROM sales.customers;

Show total number of customers

SELECT count(*) FROM sales.customers;

Show transactions for Chennai market (market code for chennai is Mark001)

SELECT * FROM sales.transactions where market_code='Mark001';

Show distrinct product codes that were sold in chennai

SELECT distinct product_code FROM sales.transactions where market_code='Mark001';

Show transactions where currency is US dollars

SELECT * from sales.transactions where currency="USD";

Show transactions in 2020 join by date table

SELECT sales.transactions.*, sales.date.* FROM sales.transactions INNER JOIN sales.date ON transactions.order_date=date.date where date.year=2020;




## Steps Followed in this project

1. Learned about AIMS grid for project planning.
2. Used MySQL for retrieving the data from the database into Power BI.
3. Data Cleaning in power query.
4. Performed ETL process (Extract Transform and Load)
5. Created measure for needs and used them for creating visuals in PowerBi.
6. In the currency there were two types of currencies in transactions, performed currency conversion to make all the currency type same
7. Data Validation
8. Data Modelling and Visualization.


###  Insights
  
1. In this dashboard, we can see company has generated total revenue in 4 years ₹ 985M, total profit margin ₹24.7M, Profit margin% 2.5%, Sales Qty ₹2M.
   in 2020 company has generated total revenue of ₹ 142M by selling a total of 350K and earned a profit of ₹ 2.1M.
2. In 4 years Delhi NCR is our largest market in terms of revenue with ₹ 520M and total contribution of 52.8% with total revenue but if you look at the profit            margin Delhi NCR is generating only 2.3% profit margin.
3. If we check the profit margin then here In 2020 Bhubaneshwar comes into the picture which is generating the highest profit margin of 10.48%. Similarly, if we can      check the Profit Contribution % by Market then here Mumbai is the largest player with 23.89% of total contribution in total profit.
4. In 4 years Bengaluru generating the lowest profit margin of -20.8%.if we can check the Profit Contribution % by Market then here also Bengaluru is the Lower with      -0.3% of total contribution in total profit.
5. In our top 5 customers, the Electricalsara Stores is our biggest customer who has generated total ₹ 413 M revenue generated in 4 years.
6. In our top 5 products,the Prod318 is our highest product has generated total  ₹ 69M revenue generated in 4 years.
7. In product type Distribution has generated the revenue of ₹494M and ownbrand revenue is ₹494M generated in entire 4 years.
7. Revenue Trend is showing that in June 2020 revenue has been decreased drastically compared to the revenue last year and the profit margin was the least in              April 2020.
  
### Key Learnings

1. Learned about what real business data sets look like.
2. Learned about how to write some major analysis queries in MySQL.
3. how to connect the database’s tables to Power Bi and how to clean & modify the unwanted data in Power Query.
4. Learned about some major practical DAX functions and measures.
5. Learned about some major analytical visuals and reports.







