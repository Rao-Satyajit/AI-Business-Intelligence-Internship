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

## Prompt

Act as a Senior BI Consultant. Review these four dashboard pages (Executive Summary, Sales Analysis, Customer Insights, Product Performance). Score the overall report out of 10. Identify 5 specific things that are unclear, cluttered, or could confuse a stakeholder, and suggest a concrete fix for each. Then suggest more executive-friendly rewrites for any chart or page title that sounds too technical.

## AI Response

Overall Score: 8/10

1. Executive Summary could be more polished
    Some KPI cards may show too many decimal places.
    Fix: Round values and use appropriate display units such as K/M.
2. Sales Analysis table is slightly cluttered
    The table contains many rows and long decimal values.
    Fix: Reduce decimal places and keep the most important fields visible.
3. Some chart labels are truncated
    Category, city, and other labels may not be fully visible.
    Fix: Resize visuals or use shorter titles/labels.
4. Customer Insights could have clearer emphasis
    The top-customer table is useful, but the key insight is not immediately obvious.
    Fix: Keep the Top 5 table and use a clearer title such as “Top 5 Customers by Sales.”
5. Product Performance could use clearer titles
    Some titles are descriptive but could be more executive-friendly.
    Fix: Use titles such as “Sales by Product Category” and “Profitability by Category.”

Executive-Friendly Title Suggestions

* Total Sales by Category → Sales by Category
* Total Sales by Month → Monthly Sales Trend
* Total Sales by City → Sales by City
* Profit Margin % by Category → Profitability by Category
* Total Sales by Sub-Category → Sales by Sub-Category

## Prompt

Write ten executive insights across these four dashboard pages. Each insight should name a specific number, a specific trend, and a suggested business action.

## AI Response

1. Total Sales: The business generated $12.64M in total sales, indicating strong overall sales performance. Management should focus on maintaining this momentum while identifying opportunities for further growth.
2. Total Profit: Total profit stands at approximately $1.47M, showing that the business is generating positive returns. Management should continue monitoring costs and product profitability to protect margins.
3. Consumer Segment: The Consumer segment contributes approximately $6.5M, or 51.48% of total sales, making it the largest segment. The business should prioritize customer retention and targeted promotions for this segment.
4. Corporate Segment: Corporate customers generate approximately $3.8M, or 30.25% of sales. Management should develop targeted corporate offers to increase this segment’s contribution.
5. Home Office Segment: Home Office contributes approximately $2.3M, or 18.27% of sales, making it the smallest segment. The business should explore targeted campaigns to increase Home Office spending.
6. Average Order Value: The average order value is $505.01. Management should explore cross-selling and bundled products to increase the value of individual orders.
7. Top Products: The displayed top products generate approximately $620,736 in combined sales. The business should maintain availability of these high-performing products and identify similar products with growth potential.
8. Category Sales: Technology is the highest-selling category, ahead of Furniture and Office Supplies. Management should investigate the factors driving Technology’s stronger performance and apply successful strategies to other categories.
9. Profit Margin: Technology has the highest profit margin at roughly 14%, while Furniture is around 7%. Management should review Furniture pricing, costs, and product mix to improve profitability.
10. Monthly Sales: Sales fluctuate considerably throughout the year, with November and December showing strong sales compared with weaker months such as February. Management should prepare inventory and marketing campaigns ahead of high-demand periods while strengthening weaker months.

## Prompt

Create a 10-slide executive presentation outline from these insights:

1. The company generated around $12.64M in sales and $1.47M in profit, showing good overall performance.
2. The Consumer segment generated around $6.5M, or 51.48% of total sales, making it the biggest contributor.
3. Technology has the highest sales and around a 14% profit margin, making it one of the strongest categories.
4. Furniture has a profit margin of around 7%, which is lower than Technology and Office Supplies.
5. Sales change throughout the year, with November and December being stronger months and February being one of the weaker months.

Each slide should have a clear one-line title and 3 supporting bullet points, ordered as: Title, Business Problem, Approach, Insight 1, Insight 2, Insight 3, Insight 4, Insight 5, Recommendations, Thank You/Questions.

⸻

## AI Response

Slide 1 — Global Superstore Business Intelligence

* Power BI dashboard project
* Focus on sales, profit, customers and products
* TNM Software Solutions Pvt. Ltd.

Slide 2 — Business Problem

* Understand overall business performance
* Identify the strongest customer and product areas
* Find opportunities to improve profitability

Slide 3 — Approach

* Used the Global Superstore dataset
* Cleaned and organized the data for analysis
* Built a four-page Power BI dashboard

Slide 4 — Strong Overall Performance

* Total sales reached $12.64M
* Total profit reached $1.47M
* Focus on maintaining profitable growth

Slide 5 — Consumer Segment Leads Sales

* Consumer generated around $6.5M
* Consumer represents 51.48% of total sales
* Focus on retaining and growing this customer segment

Slide 6 — Technology Is a Strong Category

* Technology has the highest sales
* Profit margin is around 14%
* Continue investing in this strong category

Slide 7 — Furniture Has Lower Profitability

* Furniture has around a 7% profit margin
* Its profitability is lower than stronger categories
* Review pricing and costs to improve margins

Slide 8 — Sales Change During the Year

* Sales vary across different months
* November and December are stronger periods
* February is one of the weaker months

Slide 9 — Recommendations

* Focus on Consumer customer retention
* Improve Furniture profitability
* Plan marketing and inventory around seasonal demand

Slide 10 — Thank You / Questions

* Thank you for your time
* Questions and discussion
* GitHub repository: https://github.com/Rao-Satyajit/AI-Business-Intelligence-Internship.git
