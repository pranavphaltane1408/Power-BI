# Report 4
# Link-- https://app.powerbi.com/view?r=eyJrIjoiNjY4NDQzZGItYzJlZS00Zjc0LWJlN2YtMWQzNTI3NjY1YWJmIiwidCI6IjJlOWI4M2I2LTI1MGYtNDY4NC05Mjc3LWVjMzc1YWIxMjMyYSJ9&pageName=e7a14bba3442e200c4c0
# Description
  The Report 4 a comprehensive personal finance tracking system that monitors income, expenses, and savings throughout 2023. It features:
	  Monthly trend analysis of expenses, income, and savings
	  Breakdown of income sources
	  Detailed expense categorization
	  Savings allocation
	  Year-over-year performance metrics
# Key Learnings :
# Income Diversification -
	1. Primary income from salary (901.2K)
	2. Secondary income from freelancing (63.0K)
	3. Total income: 964.2K
# Expense Distribution -
	1. Highest expense: House Rent (192.0K)
	2. Second highest: EMIs (124.0K)
	3. Essential expenses (Groceries & Food): 112.0K
	4. Health-related expenses: 37.0K
	5. Shopping: 22.6K
# Savings Pattern -
	1. Total savings: 539.7K
	2. Majority in liquid cash (433.5K - 80.3%)
	3. Mutual funds investment (86.0K - 15.9%)
	4. Strong saving percentage at 56%
	
# Performance Metrics - 
	1. Monthly income change: 109.2%
	2. Expense ratio: 53.3%
	3. Saving ratio: 56%

# Top 10 Questions for Analysis -

1. What factors contributed to the 109.2% month-over-month income change?
2. Why is there such a high concentration (80.3%) in liquid cash versus other investment options?
3. Is the current expense ratio of 53.3% optimal for long-term financial health?
4. How sustainable is the freelancing income stream?
5. What drove the fluctuations in expenses between Jan-Nov 2023?
6. Are the EMIs optimally structured given the income level?
7. Is the health expense allocation sufficient for comprehensive coverage?
8. How does the savings allocation between liquid cash and mutual funds compare to recommended ratios?
9. What caused the shopping expenses to be relatively low at 22.6K?
10. How does the housing rent to income ratio compare to financial planning benchmarks?

# Important DAX Formulas -
	1.Savings Percentage:
		Savings % = 
		DIVIDE([Total Savings], [Total Income], 0) * 100
		
	2.Expense Ratio:
		Expense Ratio = 
		DIVIDE([Total Expenses], [Total Income], 0) * 100
		
	3. Month over Month Income Change:

 
	4. MOM Income Change = 
		DIVIDE(
		[Current Month Income] - [Previous Month Income],
		[Previous Month Income],
		0
		) * 100
		
	5. YTD Savings:
		YTD Savings = 
		CALCULATE(
			SUM(Finance[Savings]),
			DATESYTD(Finance[Date])
		)
		
	6. Running Total Expenses:
		Running Total Expenses = 
		CALCULATE(
			SUM(Finance[Expense]),
			FILTER(
				ALL(Finance[Date]),
			Finance[Date] <= MAX(Finance[Date])
			)
		)
		
		
# Report Summary - 
The Report 4 reveals a healthy financial position with:

	1. Strong income growth (109.2% MOM change)
	2. Balanced expense management (53.3% expense ratio)
	3. Robust savings (56% savings ratio)
	4. Conservative investment approach (80.3% in liquid cash)

# Areas for potential optimization:

	1. Investment diversification (currently heavily weighted toward liquid cash)
	2. Expense optimization in housing and EMIs
	3. Potential for increasing mutual fund allocation
	4. Review of health expense adequacy
	5. Exploration of additional freelancing opportunities given its success



# Snapshot -- 

