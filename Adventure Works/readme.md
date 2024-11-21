# Adventure Works
# Description:
The Adventure Works Business Report is a comprehensive dashboard that consolidates top insights across various business dimensions, 
focusing on product performance, customer demographics, sales trends, and financial metrics from January 2015 to June 2017.

# Link -- https://app.powerbi.com/view?r=eyJrIjoiNmU4OTkwMjYtNDgyNS00NjE5LWFjZjEtZmMwNjJiNWUzMGMyIiwidCI6IjJlOWI4M2I2LTI1MGYtNDY4NC05Mjc3LWVjMzc1YWIxMjMyYSJ9&pageName=68e9c79d066008726a41

# Key Learnings:

# Product Performance


1. Top-selling subcategories include Tires and Tubes, Road Bikes, and Helmets
2. Some products have higher return rates (e.g., Classic Vest, S at 6.3%, HL Road Tire at 5.1%)
3. Total revenue and order trends show fluctuations over the reporting period


# Customer Demographics


1. Gender Distribution:

Male: 50.03%
Female: 49.3%
Not Specified: 0.68%


2. Income Level Distribution:

Average: 46.1%
Low: 40.8%
High: 11.23%


3. Occupation Distribution:

Professional: 31.49%
Skilled Manual: 23.66%
Management: 17.4%
Clerical: 15.7%
Manual: 11.66%




#Financial Insights


1. Revenue Last Month: $627.34K (13.91% above goal)
2. Total Orders: 644 (3.04% above target)
3. Return Rate: 2.2% (significantly below goal of 43%)

# Top 10 Questions to Explore:

1. What drives the high return rates for specific products like Classic Vest and HL Road Tire?
2. How can we capitalize on the strong performance of Tires and Tubes subcategory?
3. What strategies can increase sales in the High and Very High income segments?
4. How do seasonal trends impact product sales and revenue?
5. What factors contribute to the success of top-performing products like AWC Logo Cap?
6. Can we develop targeted marketing strategies for different occupational segments?
7. What explains the fluctuations in profit and adjusted profit over time?
8. How can we reduce return rates across product lines?
9. What insights can we gain from the gender and income level distribution?
10. How do regional differences (Europe, North America, Pacific) impact sales?

#Important DAX Formulas (Suggested):

1. Total Revenue Calculation:

Total Revenue = SUM(Sales[Revenue])

2. Return Rate:

Return Rate % = 
DIVIDE(
    CALCULATE(COUNT(Sales[ReturnFlag]), Sales[ReturnFlag] = 1),
    CALCULATE(COUNT(Sales[OrderID]))
) * 100

3. Profit Margin:

Profit Margin % = 
DIVIDE(
    SUM(Sales[Profit]),
    SUM(Sales[Revenue])
) * 100

4. Monthly Revenue Growth:

Monthly Revenue Growth = 
VAR CurrentMonthRevenue = CALCULATE(SUM(Sales[Revenue]), MONTH(Sales[OrderDate]) = TODAY())
VAR PreviousMonthRevenue = CALCULATE(SUM(Sales[Revenue]), MONTH(Sales[OrderDate]) = MONTH(TODAY())-1)
RETURN 
DIVIDE(CurrentMonthRevenue - PreviousMonthRevenue, PreviousMonthRevenue) * 100

5. Customer Segmentation:

Customer Segment = 
SWITCH(
    TRUE(),
    Sales[AnnualIncome] < 30000, "Low Income",
    Sales[AnnualIncome] < 60000, "Average Income",
    Sales[AnnualIncome] < 100000, "High Income",
    "Very High Income"
)


# Report Summary:
The Adventure Works Business Report reveals a robust and diverse business performance across multiple dimensions. 
The company demonstrates strong sales across various product categories, with a balanced customer base in terms of gender and a mix of income levels and occupations. 
Key strengths include exceeding revenue and order targets, maintaining a low return rate, and showing consistent revenue trends.

# Opportunities for improvement include:

1. Reducing product return rates
2. Expanding market share in high-income segments
3. Developing targeted marketing strategies
4. Investigating product-specific performance variations

# Dashboard-Snapshot --
![Screenshot (9)](https://github.com/user-attachments/assets/63c841ea-d5c7-4ed8-8280-9a5da9acb975)
![Screenshot (10)](https://github.com/user-attachments/assets/8fb410da-982c-46d6-ba2a-a99f54dc28b1)
![Screenshot (11)](https://github.com/user-attachments/assets/062419d8-8ee2-4d1e-9ca3-8e3836024903)
![Screenshot (12)](https://github.com/user-attachments/assets/9d67741e-b1c5-47a6-b10b-f41c2d0d4c0b)


