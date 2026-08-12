# AI Prompts Log

## Prompt

Act as a Senior Data Analyst. Here are the columns and sample rows from my dataset. Explain what each column likely means from a business perspective, and suggest five business questions this dataset could answer.

## AI Response

Business meaning of the columns:
- Category: Main product category.
- Sub-Category: Specific type of product.
- Customer ID: Unique customer identifier.
- Customer Name: Name of the customer.
- Product ID: Unique product identifier.
- Product Name: Product sold.
- Order ID: Unique order identifier.
- Order Date: Date the order was placed.
- Ship Date: Date the order was shipped.
- Sales: Revenue generated.
- Profit: Profit earned.
- Discount: Discount applied.
- Quantity: Units sold.
- Region, Country, State and City: Geographic location of the order.

Five business questions:
1. Which product categories generate the highest sales?
2. Which regions are the most profitable?
3. How do discounts affect profit?
4. Which customers generate the most revenue?
5. Which products perform the best?



## Prompt

Act as a Senior Data Analyst. My dataset has: all checked columns show 100% valid values with 0% errors and 0% empty values. Order ID has repeated values, with 673 distinct values and 450 unique values. Sales has no negative values, and Profit contains some negative values. For each issue, suggest whether to remove, fill, or flag the affected rows, and explain the business risk of getting it wrong.

## AI Response

Based on the data quality checks, I would recommend the following:

1. *Missing values and errors:* No missing values or errors were found in the checked columns, so there is currently nothing that needs to be removed or filled. This is good because changing valid data unnecessarily could create incorrect information.

2. *Repeated Order IDs:* The repeated Order IDs should not be removed because one order can contain multiple products and therefore appear on more than one row. Removing these rows could result in losing valid sales information.

3. *Sales values:* No negative Sales values were found, so there is no immediate need to remove or change any Sales records. Incorrectly changing sales values could affect the accuracy of revenue analysis.

4. *Negative Profit:* Negative Profit values should be kept because they can represent transactions where the business made a loss. Removing them would give an unrealistic view of the company's actual profitability.

5. *Overall recommendation:* The identified values should be reviewed during the cleaning stage rather than automatically removed. The main risk is that removing valid records could lead to inaccurate sales and profit analysis.


## Prompt

Design a 4-page Power BI dashboard for a CEO and their team, using these KPIs: Total Sales, Total Profit, Total Orders, Average Order Value, Profit Margin, and these dimensions: Region, Category, Product, Customer, Date. Page 1 is an Executive Summary, Page 2 is Sales Analysis, Page 3 is Customer Insights, Page 4 is Product Performance. For each page, suggest which visuals fit and where they should sit.

## AI Response

Page 1 — Executive Summary

Purpose: Give the CEO a quick overview of overall business performance.

KPIs:

* Total Sales
* Total Profit
* Total Orders
* Average Order Value

Suggested layout:

* Place four KPI Card visuals across the top.
* Place a Line Chart below the cards showing Total Sales over time using Date/Month.
* Place a Map showing Total Sales by Region or Country.
* Place Region and Date/Year slicers on the left or top for easy filtering.

Main question answered: How is the business performing overall, and how are sales changing over time and across regions?

Page 2 — Sales Analysis

Purpose: Understand sales performance by category, region, and time.

Suggested layout:

* Clustered Column Chart showing Total Sales by Category.
* Line Chart showing Total Sales over time, with Category as the legend.
* Table showing Region, Total Sales, Total Profit, and Average Order Value.
* Copy the Region and Date/Year slicers from Page 1.

Main question answered: Which categories and regions are performing best, and how are sales changing over time?

Page 3 — Customer Insights

Purpose: Understand the most valuable customers and customer segments.

Suggested layout:

* Table showing the Top 5 Customers by Total Sales.
* Donut Chart showing Total Sales by Customer Segment.
* Card showing Average Order Value.
* Clustered Bar Chart showing Total Orders by Customer Segment.

Main question answered: Which customers and customer segments contribute most to sales and orders?

Page 4 — Product Performance

Purpose: Identify the best-selling and most profitable products and categories.

Suggested layout:

* Table showing the Top 10 Products by Total Sales.
* Bar Chart showing Profit Margin % by Category.
* Treemap or Clustered Column Chart showing Total Sales by Sub-Category.

Main question answered: Which products and categories generate the most sales, and which are the most profitable?

Overall Dashboard Design

All four pages should use a consistent theme, font style, title format, and visual alignment. KPI cards should be placed near the top of relevant pages so important numbers are immediately visible. Slicers should be placed consistently, and visuals should be aligned neatly to make the dashboard easy for a CEO or manager to understand and use.
