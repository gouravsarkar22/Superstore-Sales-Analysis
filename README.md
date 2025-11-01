# Superstore-Sales-Analysis
An end-to-end business intelligence project analyzing 10,000+ retail transactions using Python and SQL to uncover actionable insights on sales performance, customer behavior, and profitability trends.


# Project Overview
This project demonstrates a complete data analytics workflow from raw data ingestion to attractive visualization creation. Built using the *Superstore Sales dataset*, it showcases skills in:

 ## Data Preprocessing 
  Worked on how to perform pre-processing of data and working on handling null values, deletion or transformation of irrelevant values, data type transformation, removing duplicates and data validations to get refined and cleaner data to perform further analysis.

Steps to perform Data Pre-processing:

Step 1: Removing duplicate rows ( there could be duplicate rows excluding Row_ID column ).

Step 2 : Converted date columns to datetime format.

Step 3: Removing rows for which few values are missing.

Step 4: Remove irrelevant values from each column if any. Validation of all values for a column( order date and ship date value must be in correct date format ). For each entry in dataset ship date >= order date.

Step 5: Export the cleaned dataset as a .csv file.

##  Exploratory Data Analysis using SQL

Load the preprocessed data and then connect to a local SQLite database *superstore_sales.db*, then worked on performing data analysis on the pre-processed data from the previous module and conducting Data Analysis using SQL. You will generate queries for given problem statements.

1. *Sales Trend Analysis* : Consistent YoY growth with seasonal peaks in Q4.
2. *Product Performance* : Technology has highest revenue but Office Supplies has better margins.
3. *Customer Segmentation* : Corporate segment has 22% higher average order value.
4. *Discount Impact* : Heavy discounting (>30%) results in negative margins.

# Business Objectives
-> Analyze sales trends and identify growth patterns.

-> Evaluate product and category profitability.

-> Segment customers based on purchasing behavior.

-> Understand geographic sales distribution.

-> Optimize shipping strategies.

-> Assess discount impact on profit margins.

# Key Insights
## Business Metrics
1. Total Revenue: $2.3M
2. Total Profit: $286K
3. Profit Margin: 12.47%
4. Total Orders: 9994
5. Unique Customers: 793
6. Products Sold: 1862

## Top Performers
1. Best Category: Technology ($836K)
2. Best Segment: Consumer (51% of sales)
3. Best Region: West ($725K)
4. Top State: California ($457K)
5. Best Ship Mode: Standard (5968 orders)

## Critical Findings
1. *Furniture Profitability Issue*: Tables and Bookcases sub-categories showing **negative profit margins** (-$17.7K total loss)
2. *Discount Impact*: Orders with **30%+ discounts** have **-12% profit margin** vs **25%** for non-discounted items.
3. *Customer Concentration*: Top **10% of the customers** cintribute **35% of total revenue.
4. *Regional Disparity*: Southern region has the **lowest profit margin** at 12.3% (requires investigation)
5. *Shipping Efficiency*: Same-day shipping used in only **5% of orders** despite premium pricing oppurtunity.
6. Philadelphia shows a promising upward trajectory, contrasting with the relatively stagnant sales in Houston and San Antonio.
7. New York City and Los Angeles dominate in product quantities across all categories.
8. Binders, Paper, and Furnishings are consistently popular across California, New York, and Washington.

## Geographic Distribution
**Top 5 states by Revenue:**
1. California - $457K
2. New York - $310K
3. Texas - $170K
4. Washington - $138K
5. Pennsylvania - $116K

## Top Performing Sub-Categories

<img width="853" height="600" alt="image" src="https://github.com/user-attachments/assets/4c4d7856-01b5-4735-a8ef-5761833b24a4" />

1. Phones, Chairs, and Storage are the top three sub-categories in sales.
2. Binders, Machines, and Tables sub-categories have the highest discount rate, which might impact their profitability.
3. Labels, Paper, and Envelopes are the most profitable sub-categories, which indicates that the cost of goods sold was lucrative for those products.

## Monthly Revenue Trend By Year

<img width="1031" height="547" alt="image" src="https://github.com/user-attachments/assets/f679fe22-fcec-40c1-8120-753f2fcc1fa6" />


1. Q4 seems to be most profitable period over the years and stays consistent.
 
2. Sales across all segments had increased year-over-year, with the Consumer segment leading the growth. The Home Office segment was smaller, yet it showed a significant increase in sales in 2022. Profit trends mirror the sales trends, but it's noteworthy that the Corporate segment's profit in 2022 didn't grow proportionally to its sales.

## Shipping Mode

<img width="859" height="547" alt="image" src="https://github.com/user-attachments/assets/fd736e42-c4a3-44fb-987a-de167be8377a" />



 Standard Class remains the dominant shipping mode in terms of sales and profit, takes generally 5 days for shipping, whereas first-class shipping naturally takes 2 and a half day for shipping.
 
 However, while sales for Standard Class increased in 2022, its profit decreased. First Class and Second Class have seen substantial growth in 2022.

## Profit Margin By Discount Category


<img width="853" height="682" alt="image" src="https://github.com/user-attachments/assets/0e4cb2b1-1d50-4458-9c55-250f2e7990f1" />



1. Giving 30%+ discount mostly backfires.
2. Upto 20% discount still plays a good role between customer retention and generating revenue.
3. Most of the order have been placed when there is no discount.

## Dashboards 

<img width="762" height="426" alt="Screenshot 2025-11-01 194437" src="https://github.com/user-attachments/assets/6179472c-6527-4dd0-bb2f-7a009ddcde07" />


























<img width="849" height="476" alt="Screenshot 2025-11-01 202945" src="https://github.com/user-attachments/assets/bddd7731-5477-48a7-bf88-626437004094" />







# Business Recommendations
Based on the analysis, here are actionable recommendations:


## 🔴 Immediate Actions
1. *Review Furniture Pricing Strategy*:
   1. Tables and Bookcases consistently unprofitable
   2. Considewr discontinuing or repricing these items
   3. Potential savings $17.7K annually

2. *Optimize Discount Policy*:
   1. Cap maximum discount at 20%
   2. Target discounts only for slow-moving inventory
   3. Potential margin improvement: 5-7%

3. *Investigate Southern Region Performance*:
   1. Lowest profit margin (12.3%)
   2. Audit operational costs and shipping expenses
   3. Align with Western region best practices


## 🟡 Short-term (3-6 months)
1. *Customer Retention Program*:
   1. 45% are one-time buyers
   2. Implement loyalty rewards for repeat purchases
   3. Focus on Corporate segment (highest AOV)

2. *Same-Day Delivery Marketing*:
   1. Only 5% adoption rate
   2. Promote to high-value customers
   3. Premium pricing oppurtunity


## 🟢 Long-Term (6-12 months)
1. *Expand Product Mix in Technology*:
   1. Highest revenue category with good margins
   2. Oppurtunity for private label products
   3. Cross-sell accessories

2. *Geographic Expansion*:
   1. Western region most profitable
   2. Replicate success in underperforming regions
   3. Focus on California and New York markets
