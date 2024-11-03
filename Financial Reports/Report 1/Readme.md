
# Financial Dashboard 
This Financial Dashboard provides a consolidated view of sales performance across multiple dimensions, 
aimed at helping executives gain top-level insights into revenue trends, regional performance, customer segments, and monthly revenue fluctuations 
over the period from 2017 to 2020.
# Link -- https://app.powerbi.com/view?r=eyJrIjoiMDIxMjdkNWQtZjc3Yy00Njg1LWFhMWMtOWYyNDg0OGNlYmZmIiwidCI6IjJlOWI4M2I2LTI1MGYtNDY4NC05Mjc3LWVjMzc1YWIxMjMyYSJ9&pageName=a0349265d756cc079c96

# Key Learnings
# Sales Performance
1. Total Revenue: $413.7M across all regions, with sales quantity reaching 1.0M units.
# Regional Revenue Breakdown:
1. Top regions include 
	(a) Delhi NCR ($220.9M), 
	(b) Mumbai ($63.0M), and 
	(c) Ahmedabad ($55.8M).
# Revenue by Zone:
1. North Zone: $287M, 
2. Central Zone: $108M, 
3. South Zone: $19M.
# Revenue by Customer Type:
1. Brick & Mortar: $308M
2. E-Commerce: $106M
# Monthly Revenue Fluctuations:
# Peak months in revenue include 
	January ($42.5M), 
	March ($39.5M), and 
	June ($38.2M).
# Top 10 Questions to Explore
1. What drives the higher revenue in regions like Delhi NCR and Mumbai?
2. How does each zone contribute to overall profitability?
3. What factors are impacting the differences between Brick & Mortar and E-Commerce revenue?
4. Which customer segments are most profitable across zones?
5. How can we increase sales in underperforming regions like the South Zone?
6. What are the reasons behind the fluctuations in monthly revenue?
7. How can we optimize sales strategies during peak revenue months?
8. Are there product-specific insights driving regional performance?
9. What are the emerging trends in revenue by customer type?
10. How can we leverage high-performing regions to improve sales in other areas?
# Important DAX Formulas : 
1.Total Revenue Calculation:
Total Revenue = SUM(Sales[Revenue])

2. Revenue by Region:
Revenue by Region = CALCULATE(SUM(Sales[Revenue]), Sales[Region] = "RegionName")

3. Revenue by Zone:
Revenue by Zone = SUMMARIZE(
    Sales,
    Sales[Zone],
    "ZoneRevenue", SUM(Sales[Revenue])
)

4. Monthly Revenue:
Monthly Revenue = CALCULATE(SUM(Sales[Revenue]), MONTH(Sales[OrderDate]) = MonthNumber)

5. Customer Type Revenue:
Customer Type Revenue = 
CALCULATE(SUM(Sales[Revenue]), Sales[CustomerType] = "CustomerTypeName")

# Report Summary
The Financial Dashboard offers a high-level perspective on sales performance, regional insights, and monthly revenue trends. 
Notable strengths include robust revenue in high-performing regions and a significant contribution from Brick & Mortar stores. 
E-Commerce remains an area with growth potential. Key opportunities include enhancing sales strategies in underperformin g zones and capitalizing 
on insights from top regions to improve overall revenue. This dashboard provides a solid foundation for making strategic decisions to 
drive growth across all dimensions of the business.

# Snapshot -- 





