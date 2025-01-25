Objective:
Analyze pizza sales data to generate key performance indicators (KPIs), identify sales trends, and provide actionable insights using SQL and Power BI.

Tools Used:
SQL (queries for extracting and analyzing data)
Power BI (interactive dashboard creation and visualization)

KPI Metrics: Calculated key business metrics, including Total Revenue, Average Order Value, and Total Pizzas Sold.

Trend Analysis: Identified daily and monthly order trends.

Category Insights: Evaluated sales distribution by pizza category and size.

Top/Bottom Analysis: Ranked pizzas by revenue, quantity sold, and order count.

Example SQL Queries:

Total Revenue:
SELECT SUM(total_price) AS Total_Revenue FROM pizza_sales;

% Sales by Pizza Category:
SELECT pizza_category, CAST(SUM(total_price) AS DECIMAL(10,2)) as total_revenue, 
CAST(SUM(total_price) * 100 / (SELECT SUM(total_price) FROM pizza_sales) AS DECIMAL(10,2)) AS PCT
FROM pizza_sales
GROUP BY pizza_category;

Interactive Dashboard in Power BI:
Created a visually appealing dashboard to present KPIs, category-level insights, and trend analyses.
Enabled filtering by pizza category, size, and time periods for dynamic insights.
Designed intuitive visuals, such as bar charts, line graphs, and percentage breakdowns.

Results:
Provided actionable insights into customer preferences and sales trends.
Highlighted the best-performing pizza categories and identified areas for improvement.

Skills Demonstrated:
Advanced SQL querying for data extraction and analysis.
Data visualization and storytelling with Power BI.
Ability to derive insights from raw data to inform business decisions.

