# Report 2
# Link -- https://app.powerbi.com/view?r=eyJrIjoiM2NjZjk0M2YtYTBkNi00Y2E5LTg4NTMtYTA1YjVmNDhjZmJiIiwidCI6IjJlOWI4M2I2LTI1MGYtNDY4NC05Mjc3LWVjMzc1YWIxMjMyYSJ9&pageName=299094f345013cebe493
# Description :
This Report 2 provides key insights into financial performance, including revenue trends, occupancy rates, 
and realization percentages across various booking platforms and property categories. 
The analysis covers metrics like RevPAR (Revenue Per Available Room), ADR (Average Daily Rate), 
and Occupancy Percentage for both weekdays and weekends, segmented by booking platform and property.

# Key Learnings
# Revenue and Occupancy Performance
	 Total Revenue: $1.69 billion.
# Occupancy Rate:
	Weekday: 51.3%
	Weekend: 73.9%
# Average Realization and ADR:
# Realization: 80.2%
# ADR: $12,696 (weekday) and 
	   $12,724 (weekend)
# Revenue by Category:
	1. Luxury: 61.62% of total revenue
	2. Business: 38.38% of total revenue
# Platform-Specific Insights
Highest Realization and ADR: Platforms like "direct online" and "makeyourtrip" show higher realization percentages and ADR, 
indicating potential for optimizing these channels.

# Revenue Trends by Month:
	Peak months and seasonal fluctuations observed for metrics like RevPAR, ADR, and Occupancy.
# Top 10 Questions to Explore:
1. Which factors drive higher occupancy on weekends compared to weekdays?
2. How can we optimize booking platforms with lower realization percentages?
3. What strategies can increase revenue in the Business category?
4. How do monthly trends in RevPAR, ADR, and Occupancy affect overall profitability?
5. Which booking platforms yield the highest return in terms of ADR?
6. How can we further leverage platforms with high realization and ADR for increased revenue?
7. What explains variations in occupancy across different property categories?
8. How can the realization rate be improved for underperforming properties?
9. What are the main factors impacting ADR fluctuations by booking platform?
10. Which seasonal patterns significantly affect revenue across properties?

# Important DAX Formulas
1. Total Revenue Calculation:

Total Revenue = SUM(Finance[Revenue])

2. Occupancy Rate Calculation:
Occupancy Rate % = 
DIVIDE(
    SUM(Finance[OccupiedRooms]),
    SUM(Finance[TotalRooms])
) * 100

3. Average Daily Rate (ADR):

ADR = DIVIDE(SUM(Finance[Revenue]), SUM(Finance[OccupiedRooms]))

4. Revenue by Category:

Revenue by Category = 
CALCULATE(SUM(Finance[Revenue]), Finance[Category] = "CategoryName")

4. Realization Percentage:

Realization % = 
DIVIDE(SUM(Finance[RealizedRevenue]), SUM(Finance[Revenue])) * 100

# Report Summary : 
The Financial Dashboard highlights strong performance metrics in luxury categories and specific booking platforms with high realization rates. 
Weekends consistently outperform weekdays in occupancy, and direct booking channels show higher ADR, suggesting strategic areas for optimization. 
Seasonal and monthly trends provide actionable insights for maximizing RevPAR and ADR during peak times. Opportunities for improvement include 
enhancing realization rates across all platforms and increasing revenue in the business category to balance the luxury segment's dominance. 
The dashboard serves as a valuable tool for data-driven decision-making, promoting growth and efficiency across financial dimensions.

# Sanpshots -- 
![Screenshot (15)](https://github.com/user-attachments/assets/f144bc95-e6f1-4e4d-b99b-e01152c580c5)
![Screenshot (16)](https://github.com/user-attachments/assets/ba53c9fb-5925-4b6a-b341-e3fe0a247c48)








