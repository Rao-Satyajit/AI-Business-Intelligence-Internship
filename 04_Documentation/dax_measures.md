# DAX Measures

## Total Sales
Formula: Total Sales = SUM('Global Superstore'[Sales])
Calculates the total sales amount.

## Total Profit
Formula: Total Profit = SUM('Global Superstore'[Profit])
Calculates the total profit generated.

## Total Orders
Formula: Total Orders = DISTINCTCOUNT('Global Superstore'[Order ID])
Counts the number of unique orders.

## Average Order Value
Formula: Average Order Value = DIVIDE([Total Sales], [Total Orders])
Calculates the average sales value per order.

## Profit Margin %
Formula: Profit Margin % = DIVIDE([Total Profit], [Total Sales])
Calculates profit as a percentage of total sales.
