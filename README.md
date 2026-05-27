Overview

This Power BI report is a sales/revenue KPI scorecard using theLook eCommerce dataset. The goal is to give a clean, “business-style” view of performance over time and which product categories are driving results.

What’s included
KPI Cards
Total Revenue
Orders
Customers
AOV (Average Order Value)
Gross Profit
Gross Margin %
Return Rate
Repeat Rate
Repeat Customers
Visuals
Total Revenue by Year (trend)
Gross Profit by Year (trend)
Top Categories by Gross Profit (bar)
Revenue Share by Category (donut)
Year slicer for quick time filtering
Data & model (high level)

Built from theLook CSV extracts (typical tables):

orders, order_items (transactions)
products (category/department/price/cost)
users (customer attributes)
optional: inventory_items, events, distribution_centers

Relationships follow the standard star-ish approach:

orders → order_items (by order_id)
order_items → products (by product_id)
orders → users (by user_id)
Notes / assumptions
If the most recent year looks “low,” it may be a partial year depending on the dataset extract.
KPI totals change with slicers/filters (expected behavior).
How to use
Download the .pbix
Open in Power BI Desktop
Use the Year slicer (and any other filters) to explore trends and category mix

Next improvements (if I extend it)
A dedicated Customer Retention page (new vs returning customers over time, cohort retention)
Product-level drill-down (Top 10 products by profit/revenue, return rate by category/brand)
Add a Date table + month/quarter slicers for smoother time analysis
