# Atliq-Hardware-dashboard-
1. Project Title / Headline

Sales Analytics: Atliq Hardware Revenue & Profit Insights Dashboard

An interactive Power BI dashboard designed to analyze sales performance, revenue trends, profit margins, and market contribution across multiple regions.

2. Short Description / Purpose

The Sales Insights Dashboard is a dynamic and analytical Power BI report built using sales data of Atliq Hardware.

This dashboard helps stakeholders monitor revenue, sales quantity, and profit margins, while identifying top-performing markets, customers, and products for better business decision-making.

3. Tech Stack

The dashboard was built using the following tools and technologies:

• SQL (MySQL) – Used for querying and extracting relevant data
• Power BI Desktop – Used to build interactive dashboard and visuals
• Power Query – Data cleaning and transformation layer
• DAX (Data Analysis Expressions) – Used for calculated measures like profit margin and revenue contribution
• Data Modeling – Relationships between tables (customers, transactions, markets, products, date)

4. Data Source
   
Source: Public dataset inspired by Atliq Hardware sales data.

The dataset includes:

• Customer data
• Product data
• Market data
• Transaction records
• Date table

It contains multi-year sales data (2017–2020) across different Indian markets.

5. Features / Highlights

• Business Problem
• Goal of the dashboard
• Walkthrough of key visuals
• Business impact & insights

Business Problem

Businesses generate large volumes of sales data but often struggle to extract meaningful insights.

Key challenges include:

• Understanding which markets drive the most revenue
• Identifying profitable vs low-performing regions
• Tracking sales trends over time
• Identifying high-value customers and products

Goal of the Dashboard

The goal is to provide a centralized and interactive dashboard that enables:

• Monitoring of total revenue and sales quantity
• Analysis of profit margins across markets
• Identification of top customers and products
• Tracking revenue trends over multiple years          

Walkthrough of Key Visuals
🔹 KPI Cards

Displays key business metrics:

• Total Revenue (₹985M / ₹336M)
• Total Sales Quantity (2M / 847K)
• Total Profit (10.49M)

These KPIs provide a quick overview of overall business performance.

🔹 Revenue by Market (Bar Chart)

Shows revenue contribution from different markets such as:

• Delhi (Highest contributor ~₹520M)
• Mumbai
• Ahmedabad
• Bhopal

🔹 Sales Quantity by Market

Displays total sales quantity across regions.

🔹 Revenue Trend (Line Chart)

Shows revenue trend across years (2017–2020).

• Revenue fluctuations over time
• Peak sales periods
• Declining trends in later periods

🔹 Top 5 Customers by Revenue

Highlights major revenue contributors like:

• Electricalsara Stores
• Electricalslytical
• Excel Stores

🔹 Top 5 Products by Revenue

Shows best-performing products such as:

• Prod040
• Prod159
• Prod065

🔹 Profit Margin Analysis

Includes:

• Revenue contribution % by market
• Profit margin contribution %
• Profit % by market
• High-profit markets
• Low-margin regions
• Profitability distribution

🔹 Customer-Level Profit Table

Detailed table showing:

• Revenue
• Revenue contribution %
• Profit margin contribution %
• Profit %

Data Analysis Using SQL

SQL was used to extract and analyze data from the database.

Key operations performed:

• Data retrieval using SELECT statements
• Filtering using WHERE conditions
• Aggregation using SUM() and COUNT()
• Joining tables using INNER JOIN
• Time-based analysis using date table

Data Transformation (Power BI)

Data cleaning and transformation performed using Power Query.

Currency Normalization
= Table.AddColumn(#"Filtered Rows", "norm_amount",
each if [currency] = "USD" or [currency] ="USD#(cr)"
then [sales_amount]*75
else [sales_amount])

Business Impact & Insights

- Market Insights
Delhi contributes the highest share of revenue.

- Revenue Trends
Revenue shows fluctuations with a declining pattern in recent periods.

- Customer Insights
A small number of customers contribute to a large portion of revenue.

- Product Insights
Top 5 products generate significant revenue share.

- Profitability Insights
Profit margins vary across markets, highlighting areas for improvement.

6. Screenshots / Demos
Show what the dashboard looks like. -
![Dashboard Preview 1](https://github.com/ShailendraBhati/Atliq-Hardware-dashboard-/blob/main/Snapshots%20of%20dashbord.png)
![Dashboard Preview 2](https://github.com/ShailendraBhati/Atliq-Hardware-dashboard-/blob/main/Snapshots%20of%20dashbord%202.png)
![Dashboard Preview 3](https://github.com/ShailendraBhati/Atliq-Hardware-dashboard-/blob/main/Snapshots%20of%20dashbord%203.png)
![Dashboard Preview 4](https://github.com/ShailendraBhati/Atliq-Hardware-dashboard-/blob/main/Snapshots%20of%20dashbord%204.png)
