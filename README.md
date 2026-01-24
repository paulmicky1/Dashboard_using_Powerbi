Power BI Sales Analytics Dashboard

Overview

This repository contains a comprehensive Power BI sales analytics dashboard that provides multi-dimensional insights into business performance across products, geographic regions, and time periods. The dashboard is designed to help stakeholders make data-driven decisions through interactive visualizations and detailed metrics.

Dashboard Summary
Key Performance Indicators (KPIs)
The dashboard tracks the following primary metrics:

Total Revenue: $24.91M
Total Cost: $14.46M
Total Profit: $10.46M
Total Orders: 25K
Return Rate: 2.17%


Dashboard Pages
1. Executive Dashboard
Executive Dashboard Overview

<img width="1295" height="778" alt="image" src="https://github.com/user-attachments/assets/3c1406b3-1f00-4c35-a408-2128f93ffb6a" />

The Executive Dashboard provides a high-level view of business performance with the following components:
Key Metrics

Four prominent KPI cards displaying Total Revenue, Total Profit, Total Orders, and Return Rate
Month-over-month performance indicators with percentage changes

Total Revenue by Year and Month

Line chart showing revenue trends from January 2020 to July 2022
Includes a confidence interval band for forecasting
Shows steady growth with notable acceleration starting in mid-2021

Total Orders by CategoryName

Horizontal bar chart displaying order volume by product category:

Accessories: ~20K orders (highest)
Bikes: ~15K orders
Clothing: ~5K orders (lowest)



Top Ten Products Table
Displays the best-performing products with columns for:

Product name
Total orders
Total revenue
Return rate percentage

Notable products include:

Water Bottle - 30 oz. (3,983 orders, $39,755.33 revenue, 105% return rate)
AWC Logo Cap (2,062 orders, $35,882.07 revenue, 59.81% return rate)
Fender Set - Mountain (1,975 orders, $87,040.80 revenue, 73.59% return rate)

Monthly Performance Cards
Three cards showing current month vs. previous month:

Monthly Revenue: 43.34K (↑2.44% from previous month: 42.31K)
Monthly Orders: 51 (↓99.88% from previous month: 42.31K)
Monthly Returns: 5 (↓54.55% from previous month: 11)

Product Type Analysis

Most Ordered Product Type: Tires and Tubes
Most Returned Product Type: Tires and Tubes


2. Map View
<img width="1305" height="793" alt="image" src="https://github.com/user-attachments/assets/6a35dc33-44ff-4339-8a0f-87fae5abe67d" />

Geographic Map View
The Map View provides geographic distribution of orders across three main regions:
Regional Filters

Select all
Europe
North America
Pacific

Geographic Visualization

Interactive world map with bubble indicators showing order concentration
Major markets highlighted:

North America: Largest bubble (United States)
Australia: Visible presence in Pacific region
Europe: Activity indicated in European region



Total Orders Display

Central metric showing 25K total orders

<img width="1305" height="793" alt="image" src="https://github.com/user-attachments/assets/f46c8eae-ed72-4f08-9809-19310d5c2eaa" />

Map with Regional Bubbles

3. Decomposition Tree
<img width="1295" height="792" alt="image" src="https://github.com/user-attachments/assets/69a6ee42-004c-4a05-a42e-19b7bbb4b10f" />

Decomposition Tree View

The Decomposition Tree allows for hierarchical analysis of orders with drill-down capabilities:
Hierarchy Levels

Total Orders: 25,164
Continent Level:

North America: 11,724 orders
Europe: 7,380 orders
Pacific: 6,060 orders


Country Level (North America expanded):

United States: 8,700 orders
Canada: 3,024 orders


Category Level (under United States):

Accessories: 6,107 orders
Bikes: 4,487 orders
Clothing: 2,534 orders


Subcategory Level (under Clothing):

Jerseys: 1,098 orders
Caps: 638 orders
Gloves: 502 orders
Shorts: 485 orders
Socks: 231 orders
Vests: 214 orders


Product Level (under Vests):

Classic Vest, L: 75 orders
Classic Vest, S: 72 orders
Classic Vest, M: 67 orders



Current Filter Context

Continent: North America
Country: United States
CategoryName: Clothing
SubcategoryName: Vests

<img width="1295" height="792" alt="image" src="https://github.com/user-attachments/assets/7017c4be-23f4-4983-8fdd-39cc88cbcbec" />


4. Product Detailed Analysis
<img width="1296" height="783" alt="image" src="https://github.com/user-attachments/assets/0fe4995f-e5ac-4d02-8f26-5533ab87e542" />

Product Detailed View

This page provides in-depth analysis of individual product performance with interactive filters and what-if analysis capabilities.
Product Selection

Dropdown to select specific products (currently showing: Water Bottle - 30 oz.)

Current Product Metrics (Water Bottle - 30 oz.)

Total Orders: 25K with previous month comparison showing 23K
Total Revenue: 24.91M (range: 0.00M to 49.83M)
Total Profit: 10.46M (range: 0.00M to 20.92M)

Price Adjustment Simulator

Interactive slider for "Price Adjustment(%)"
Currently set to 0.70 (70%)
Allows users to model impact of pricing changes

Product Metric Selection
Checkboxes to filter displayed metrics:

☐ Total Orders
☐ Total Revenue
☐ Total Profit
☐ Total Returns
☑ Return Rate (currently selected)

Adjusted Profit and Total Profit by Year

Dual-line chart comparing:

Adjusted Profit (light blue line): Shows projected profit with price adjustments
Total Profit (dark blue line): Shows actual historical profit


Timeline: 2020 to 2022
Both metrics show steady upward trend
Adjusted Profit reaches ~10M by 2022
Total Profit reaches ~4M by 2022

Return Rate by Year

Area chart showing return rate trends from 2020 to 2022
Return rate starts at ~3.0% in 2020
Decreases to ~2.0% by 2022
Consistent downward trend indicating improving product quality or customer satisfaction

Key Insights Panel
Text analysis showing:

"Adjusted Profit (45.64% increase) and Total Profit (49.49% increase) both trended up between 2020 and 2022."
"Across all metrics, Adjusted Profit had the most interesting recent trend and started trending up on 2020, rising by 45.64% (3,233,787.75) in 2 years."
"Adjusted Profit jumped from 7,085,055.84 to 10,318,843.59 during its steepest incline between 2020 and 2022."
"Total Profit experienced the longest period..." (text continues)



Data Model
Key Dimensions

Geography: Continent → Country → Region
Products: Category → Subcategory → Product
Time: Year → Month → Day

Key Measures

Revenue metrics (Total Revenue, Monthly Revenue)
Profit metrics (Total Profit, Adjusted Profit)
Order metrics (Total Orders, Monthly Orders)
Return metrics (Total Returns, Return Rate)
Cost metrics (Total Cost)


Features
Interactive Capabilities

Cross-filtering: Selections in one visual filter related visuals
Drill-down/Drill-up: Navigate hierarchies in decomposition tree
What-if Analysis: Simulate pricing scenarios and their impact
Geographic Filtering: Filter by continent/region
Time-based Analysis: Track trends over time periods
Product Comparison: Compare performance across products

Navigation

Tab-based navigation between dashboard pages:

Executive Dashboard
Map
Decomposition Tree
Product Detailed



Back button for returning to previous views
Page navigation controls (< >)


Key Insights
Performance Highlights

Strong Profitability: 42% profit margin ($10.46M profit on $24.91M revenue)
Low Return Rate: 2.17% return rate indicates good product quality
Growth Trajectory: Revenue shows consistent upward trend from 2020-2022
Geographic Distribution: North America leads with 46.5% of total orders
Category Performance: Accessories dominates order volume

Areas of Focus

High Return Products: Some products show return rates exceeding 100% (potentially data quality issue or replacement program)
Monthly Order Volatility: Significant month-over-month fluctuations in order volume
Category Optimization: Clothing category has room for growth compared to Accessories


Usage Instructions
For Business Users

Navigate to the Executive Dashboard for a quick business overview
Use the Map view to understand geographic distribution
Explore the Decomposition Tree to identify opportunities in specific segments
Dive into Product Detailed view for individual product analysis

For Analysts

Use filters to segment data by region, time period, or product category
Leverage the what-if analysis to model pricing strategies
Export data from visuals for further analysis
Create bookmarks for commonly used filter combinations
