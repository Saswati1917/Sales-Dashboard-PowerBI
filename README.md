# Sales-Dashboard-PowerBI
Interactive Sales Dashboard built with Power BI, DAX, and Power Query

📌 **Project Overview**

This project showcases an interactive Sales Dashboard built in Power BI to analyze product performance, sales trends, discounts, and regional demand.
The goal was to provide a 360° view of sales performance — from top-performing products and sales trends to customer-level transaction analysis — enabling businesses to make data-driven decisions.

🎯 **Business Requirements**

The dashboard was designed to answer the following key business questions:

1. Identify the Top/Bottom 5 products by Sales, Profit, and Quantity Sold.

2. Analyse Sales Trends over time (daily, monthly, quarterly, annually).

3. Show the relationship between Sales & Profit.

4. Enable comparison of Sales, Profit, and Quantity Sold between two custom time periods.

5. Display the average discount offered across discount categories.

6. Show the total number of orders.

7. Provide a detailed order-level view with filters (Product, Date, Customer, Promotion).

8. Display Sales by City/Region.

🛠️ **Data & Modeling**

Data Source: Sales transaction dataset (fact table + dimension tables for Customer, Product, Promotion, Date).

Data Cleaning & Transformation (Power Query):

1. Verified and adjusted data types

2. Merged fact and dimension tables

3. Created calculated columns: Total Sales, Discount Value, Net Sales, Profit

4. Handled nulls and blanks in promotion/discount data

Data Modelling (Star Schema):

1. One Fact table (transactions)

2. Multiple Dimension tables (Customer, Product, Date, Promotion, City)

3. Relationships: One-to-Many, single-direction filtering

📐** DAX Measures**

Some key DAX measures created for analysis:

1. Total Sales = SUM(Units Sold × Price per Unit)

2. Discount Value = (Total Sales × Discount %) / 100

3. Net Sales = Total Sales – Discount Value

4. Profit = 10% of Net Sales (for this dataset)

5. Period-over-Period Comparison → Used CALCULATE, USERELATIONSHIP, and ALL to compare metrics across two date tables

📊** Dashboard Features**
🔹 Top/Bottom Product Analysis

1. Identified top-performing products (iPhone 14, MacBook Air, Sony Bravia TV), driving revenue & profit

2. Highlighted low-contributing FMCG items (Colgate, Dove, Nivea)

🔹 Overview Dashboard

1. Sales Trends over time with drill-down (Year → Quarter → Month → Day)

2. Net Sales vs Profit scatter plot (strong linear correlation)

3. Discount Categories – Weekend Flash & Clearance Sales contributed the most

4. Sales by City – Metro cities dominate overall sales

5. Orders – Total 3,510 orders captured

🔹 Period Comparison

1. Compare Sales, Profit, and Quantity Sold dynamically between two user-selected periods

2. Helps analyse seasonal demand, promotional impact, and year-over-year growth

🔹 Order-Level Report

1. Detailed transactional view with filters (Date, Product, Customer, Promotion)

2. Allows granular analysis of customer purchase behaviour & product profitability

🔑 **Key Insights**

1. Premium electronics drive the majority of revenue and profit, while FMCG products underperform.

2. Metro cities (Delhi, Mumbai, Bengaluru, Hyderabad) dominate sales; limited penetration in smaller cities.

3. Flash & clearance campaigns significantly boost short-term sales compared to festive campaigns.

4. Dynamic period comparison enables businesses to assess performance across seasons and campaigns.

5. Granular order-level analysis supports customer-level targeting and SKU-level profitability checks.

⚙️ **Tech Stack**

Power BI Desktop – Data Modeling, Visualization, Report Building

Power Query – Data Cleaning & Transformation

DAX – Calculated Measures & Time Intelligence

Data Modelling – Star Schema design

📷 **Dashboard Screenshots**

![Top/Bottom Products](Screenshot(88).png)  
![Overview Dashboard](Screenshots(89).png)  
![Period Comparison](Screenshots(90).png)  
![Order-Level Report](Screenshots(91).png)  

🚀 **How to Use**

1. Clone/download the repository

2. Open the .pbix file in Power BI Desktop

3. Interact with the report using slicers and filters

4. Explore insights at the product, customer, and city levels

📌 **Project Outcome**

1. The dashboard provides a comprehensive view of sales performance that helps businesses:

2. Identify revenue drivers & underperforming products

3. Track sales trends and campaign effectiveness

Optimize discount strategies

Improve customer targeting and product portfolio decisions
