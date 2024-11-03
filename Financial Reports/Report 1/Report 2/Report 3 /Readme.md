# Report 3
# Link -- https://app.powerbi.com/view?r=eyJrIjoiOGU4ZTAyNzctYTE2MC00ZTU2LWJiY2QtOTNjNGI2YTQ5NmU4IiwidCI6IjJlOWI4M2I2LTI1MGYtNDY4NC05Mjc3LWVjMzc1YWIxMjMyYSJ9&pageName=a38116a7602d2ba06067
# Description 
This Report 3 provides an overview of key financial metrics, including sales revenue, cost of sales, operating expenses, 
and profit margins from 2018 to 2020. The report examines trends in gross profit, operating profit, and net profit, 
segmented across various countries, providing insights into the financial health and operational efficiency of the organization.

# Key Learnings
# Revenue and Profitability Trends
	1. Sales Revenue:
	2. Growth from $3.57M in 2018 to $7.83M in 2020.
# Gross Profit Margin:
	Consistent margins around 66.7% - 69.6% across 2018 to 2020.
# Operating Profit:
	Increased from $740.8K in 2018 to $1.52M in 2020, highlighting operational improvements.
# Net Profit:
	Grew from $623.9K in 2018 to $1.3M in 2019 but slightly decreased to $1.29M in 2020.
# Expense Analysis
	1. Operating Expenses:
		Significant increase in administration, marketing, and sales expenses over the years.
	2. Non-Operating Income:
		Includes interest income, asset sales gains, exchange gains, and dividend income, with a notable increase from $36.4K in 2018 to $72.3K in 2020.
		
# Top 10 Questions to Explore :
1. What factors contributed to the growth in sales revenue from 2018 to 2020?
2. How can we optimize operating expenses to improve profit margins further?
3. What strategies can help maintain or increase net profit after 2020?
4. How do different countries (e.g., USA, UK, Germany) contribute to overall revenue and profitability?
5. Which operational areas need investment to sustain growth in operating profit?
6. What factors are causing fluctuations in net profit, despite revenue growth?
7. How does the marketing spend correlate with sales growth year-over-year?
8. What are the primary drivers behind the increase in non-operating income?
9. How can we further optimize the cost of sales?
10. What steps can be taken to increase gross profit percentage?

# Important DAX Formulas: 


	1. Total Revenue Calculation:

	Total Revenue = SUM(Finance[Sales])

	2. Gross Profit Calculation:

	Gross Profit = SUM(Finance[Sales]) - SUM(Finance[CostOfSales])
	
	3. Gross Profit Margin:


	Gross Profit Margin % = 
	DIVIDE(SUM(Finance[GrossProfit]), SUM(Finance[Sales])) * 100
	
	4. Operating Profit Calculation:

	Operating Profit = SUM(Finance[GrossProfit]) - SUM(Finance[OperatingExpenses])
	
	5. Net Profit Calculation:

	Net Profit = SUM(Finance[OperatingProfit]) + SUM(Finance[NonOperatingIncome]) - SUM(Finance[InterestAndTax])
	
# Report Summary: 
The Financial Dashboard provides a comprehensive view of the organization’s financial growth and challenges from 2018 to 2020. 
Strong sales revenue growth and improved operating profit indicate effective operational strategies. However, rising operating expenses highlight areas 
for cost optimization to protect profit margins. Non-operating income has also increased, which supports net profit, but fluctuations in net profit 
suggest potential areas for financial control and efficiency gains. The dashboard serves as a powerful tool to drive financial strategy, focusing on 
expense control, revenue growth, and profitability improvements.

# SnapShots --
![Screenshot (17)](https://github.com/user-attachments/assets/6a2a73e2-0bb9-4f4f-ad91-ff09d0d4945c)
![Screenshot (18)](https://github.com/user-attachments/assets/7caf859c-6109-4392-874c-3bbece628a3d)

