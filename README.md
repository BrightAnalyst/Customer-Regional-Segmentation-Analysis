Project Overview
SQL filtering analysis using logical operators to segment customers by market segment and geography, revealing that 83% of customers exist outside underperforming South region.
Key Findings:

Corporate + Consumer segments = 645 customers (81.3%)
Non-South regions = 659 customers (83.1%)
Strategic focus on 3 regions retains 83% of customer base
Home Office segment represents only 18.7% of customers

🎯 Business Questions

Which market segments (Corporate vs. Consumer vs. Home Office) should we prioritize?
What is the impact of exiting the South region?
Can we focus resources on fewer segments/regions for better ROI?


Query 1: Corporate & Consumer Segments
sqlSELECT * 
FROM customer
WHERE segment = 'Corporate' OR segment = 'Consumer';
Results: 645 customers (81.3% of total)
Query 2: Excluding South Region
sqlSELECT * 
FROM customer
WHERE NOT region = 'South';
Results: 659 customers (83.1% of total)
📈 Analysis Results
Segment Distribution
SegmentCustomersPercentageConsumer~42053%Corporate~22528%Home Office14819%
Insight: Corporate + Consumer = 81.3% of customer base
Geographic Focus (Non-South)
RegionCustomers% of Non-SouthWest25538.7%East22033.4%Central18427.9%Total659100%
Insight: Excluding South retains 83.1% of customers
💡 Strategic Implications
The 83/17 Rule
83% of value comes from:

Corporate + Consumer segments (not Home Office)
West + East + Central regions (not South)

17% to reconsider:

Home Office segment (148 customers)
South region (134 customers)

Controversial Recommendation: Market Exit
South Region Financial Analysis:
Costs:

Sales team: $255K
Marketing: $180K
Office/operations: $83K
Total: $518K

Revenue: $1.14M
Gross Profit: $513K
Net Contribution: -$5K (break-even)
Recommendation: Exit South, reallocate $518K to West/East/Central
Expected Impact:

Lose 134 customers (17%)
Gain 80+ customers in strong regions
Net growth: +151 customers (+19%)

🎯 Recommendations
Segment Strategy
Double Down:

Consumer: Self-serve product, freemium model
Corporate: Enterprise features, white-glove service

Phase Out:

Home Office: Migrate to Consumer or Corporate tiers
Eliminate dedicated Home Office features

Geographic Strategy
Invest:

West: +$260K (50% of South savings)
East: +$155K (30% of South savings)
Central: +$103K (20% of South savings)

Exit:

South: 90-day transition, customer migration support

🛠️ Technical Skills

SQL Logical Operators (OR, NOT, AND)
Boolean filtering
Multi-condition WHERE clauses
Scenario modeling
Strategic data analysis

