E-Commerce Website
Churn Rate 
Data Science Problem Framing 
1.) Uncover Problem
•	What is current churn rate? 28-30%
•	Which type of customer has churn rate?
•	Since when it increased drastically? — 6 months but slight shifts were noticed before

Key Insight: A 10% jump in churn rate (28% → 38%) within 6 months signals a critical inflection point requiring immediate data-driven investigation.

2.) To Technical Department
•	What changes were made after which churn rate increased abruptly?
•	Have you done any changes in your app or delivery pattern within these 6 months?
•	Any pricing or discount strategy changes?

Suspected Changes Timeline:
–	5 months ago — Payment gateway update
–	4 months ago — App UI redesign + Delivery partner change
–	3 months ago — Discounts reduced, competitor increased offers

3.) To Management
Why this problem is important?
•	Direct contact with revenue.
•	If decrease in churn rate will remain intact then it will become a hideous situation for company.
•	Loss in this market race (because there are many active competitors)

Business Impact:
–	Acquiring a new customer costs 5x more than retaining an existing one
–	High churn = reduced Customer Lifetime Value (CLV)
–	Investors view high churn as red flag for unsustainable growth

4.) Better Approach
"Identifying the customer who can churn (Eg: new customers, if customer is inactive for more than 60 days, tier 2 customers) so that company can take actions such as - discounts, coupons etc. to keep that customer intact with themselves."

Who? Customers facing problems.
What? Predict churn rate.
Why? So that possible solution can be tried.
Outcome: 8-10% decrease in churn rate.

5.) Is AI REALLY Needed?
AI should be used for:
•	Finding patterns
•	Customer segmentation and offers according to that.
•	Insights
•	Churn detection.

In our case churn may depend upon:
•	Type of customers
•	Area
•	Poor customer services
•	If cost is higher than utility acc. to customer.
•	Change in needs of customers.

Why Not Simple Rules?
Simple rules like "if inactive 60 days = churned" miss complex patterns. AI can detect combinations — e.g. a new Tier-2 city customer who had a delivery delay + used app after UI update — that no simple rule would catch.

6.) Identifying Stakeholders
Customers:
•	Their problem can be tackled.
Sellers:
•	They will get stable tools/platform and chances of their item to get selected will increase.
Investors:
•	Will get profit
Employee:
•	Increase in productivity.
•	Manager can analyse with help of AI instead of guessing.
Founder:
•	High revenue by retaining existing customers.
•	Competitive advantage over other companies.
•	Customer insights.

7.) Define the AI Task — ML Formulation
•	Classification: either 'stay' or 'leave'.
•	Segmentation of customers: Based on customer behavior so that we can provide them alternatives to make them stay. For instance, if churn rate of one customer is low then we can provide them discounts in low amount and so on.
•	Risk scoring: first need to find that, then customer segmentation according to that.

Suggested ML Models:
–	Logistic Regression — baseline classification
–	Random Forest — feature importance for root cause
–	XGBoost — high performance churn prediction
–	K-Means Clustering — customer segmentation

8.) Determining Success Metrics
•	Accuracy
•	Precision
•	Recall
•	F1 Score
•	Etc.

Priority Metric: Recall is most important here — we want to catch as many at-risk customers as possible, even if it means some false positives. Missing a churning customer is more costly than sending an extra discount.

9. Defining Constraints
Operational Constraints:
•	Can provide discount to only few customers.
Data Constraints — Certain things may not exist:
–	Financial recalls.
–	Customer's taste of liking changes over time.
–	Limited historical data for some new customers.
–	Last 3 months data may have quality issues (system migration).
Ethical Constraints:
•	Protection of customer's details.
•	Non manipulation.

10. Determining Assumptions and Risks
Assumptions:
•	Actions will be taken according to customer's segments
•	Historic data is beneficial.
•	60-day inactivity = churned customer (to be validated)

Risks:
•	Missing data
•	Biasness in data.
•	Model may not generalise across all customer segments

This document serves as the Problem Framing Foundation for the Churn Prediction AI ML Project.
