# Business Insights 360
# Link --https://app.powerbi.com/view?r=eyJrIjoiZTRhM2FlNGEtNjFjMi00ZmY1LWIxZDAtYjI1ZmZlN2Q2M2I1IiwidCI6IjJlOWI4M2I2LTI1MGYtNDY4NC05Mjc3LWVjMzc1YWIxMjMyYSJ9&pageName=7d027c10a082c2908edc
# Description
Business Insight 360 is a comprehensive business intelligence dashboard that provides in-depth analytical views across multiple business dimensions including Finance, Sales, Marketing, and Supply Chain. The dashboard offers detailed insights into company performance, covering metrics such as Net Sales, Gross Margin, Profitability, Forecast Accuracy, and Market Share across different regions, segments, and customers.

# Top 10 Questions the Dashboard Answers
1. What is the overall Net Sales performance across different years?
2. How do different product segments contribute to the company's revenue?
3. What is the Gross Margin percentage for various product categories?
4. Which regions are performing best in terms of Net Sales and Profitability?
5. What is the Forecast Accuracy for different customers and product segments?
6. How does the company's market share compare to competitors?
7. What are the Net Profit percentages across different business segments?
8. How do different sales channels (Retailer, Direct, Distributor) perform?
9. What are the inventory risks (Excess Inventory or Out of Stock) for different customers?
10. How have key financial metrics trended over the past few years?

# Important DAX Formulas
1. Total Net Sales = SUM(Sales[Net Sales])

2. Gross Margin Percentage = 
   DIVIDE(
     SUM(Sales[Gross Margin]), 
     SUM(Sales[Net Sales])
   ) * 100

3. Forecast Accuracy Calculation = 
   CALCULATE(
     AVERAGE(Forecast[Accuracy Percentage]),
     FILTER(Forecast, Forecast[Year] = SELECTEDVALUE(Year[Year]))
   )

4. Net Profit Percentage = 
   DIVIDE(
     SUM(Financials[Net Profit]),
     SUM(Financials[Net Sales])
   ) * 100

5. Market Share Calculation = 
   DIVIDE(
     SUM(Sales[Company Sales]),
     SUM(Sales[Total Market Sales])
   ) * 100
   
# Key Learning Points
# Financial Performance:

Net Sales: ₹4,968M
Gross Margin: ₹1,436.17M
Net Profit: -₹509.13M (indicating financial challenges)


# Product Segment Insights:

Notebook segment is the largest, with ₹1,973M in Net Sales
Notebooks have the highest Net Sales but also significant losses (-12.53% Net Profit)


# Regional Performance:

APAC leads in Net Sales with ₹2,606M
North America has the highest Gross Margin percentage (30.97%)
LATAM is the only region with a positive Net Profit


# Forecast and Inventory Management:

Overall Forecast Accuracy is challenging
Many customers and segments face Out of Stock (OOS) or Excess Inventory (EI) risks


# Market Share:

Company's market share fluctuates between 47.8% and 53.6% over the years

## Overview
Comprehensive business intelligence dashboard providing deep insights into financial performance, sales, marketing, and supply chain metrics.

## Key Metrics
- Total Net Sales: ₹4,968M
- Gross Margin: ₹1,436.17M
- Net Profit: -₹509.13M

## Major Findings
- Notebook segment dominates sales but shows significant losses
- APAC region leads in Net Sales
- Forecast accuracy and inventory management need improvement

## Challenges
- Negative Net Profit across most segments
- Inventory management risks
- Fluctuating market share

## Recommendations
1. Improve profitability in key segments
2. Enhance forecast accuracy
3. Optimize inventory management
4. Focus on high-margin regions and products

## Data Sources
- Finance View
- Sales View
- Marketing View
- Supply Chain View

## Technologies Used
- Business Intelligence
- Data Analysis
- Financial Reporting

## Dashboard Snapshot -- 
![Screenshot (3)](https://github.com/user-attachments/assets/0805e921-bd99-42dd-a122-98ab6037643d)
![Screenshot (4)](https://github.com/user-attachments/assets/bdbee57b-99da-4c8b-900c-a4c30ac3bb21)
![Screenshot (5)](https://github.com/user-attachments/assets/ec8361d8-8fda-46b3-b58c-7e5a92dbc13d)
![Screenshot (6)](https://github.com/user-attachments/assets/8ef7d5b2-45a5-43c0-9c9b-813d0d6fb8d3)
![Screenshot (7)](https://github.com/user-attachments/assets/e8bd3dd6-b6a0-42aa-a8d8-f0e1b562d19f)
![Screenshot (8)](https://github.com/user-attachments/assets/3b512589-b010-4935-8205-d8bbe2696850)
