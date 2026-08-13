# procurement-supplier-analytics
Problem Statement
Real-world procurement teams 777 purchase orders across 5 suppliers manages these, but they were not having a unified way of judging:
which supplier is delivering on time ?
which supplier is sending defective products ?
which supplier is not following compilance rules
where the spend risk of company is greater ?

Without proper scoring system, procurement managers take decisions on the basis of gut feeling, whether the supplier is good or bad, which can be wrong in case having 45 million dollar spend

Given fragmented procurement data across delivery, quality, and compliance metrics, design a data-driven system to identify high-risk suppliers before they cause supply chain disruption

Solution Approach
 I made multi-factor weighted risk scoring model - combining three risk pillars
Step 1 — Data Cleaning
Step 2 — Metrics Calculate Kiye (Supplier level pe)
Avg Lead Time + Coefficient of Variation (CV)
Cancellation Rate
Defect Rate - defective units / total quantity
Compliance Rate 
Cost Savings % — negotiated price vs list price
Step 3 — Made Risk Pillars then combined
Delivery Risk = 50% Cancellation Rate + 50% Lead Time Variability
Quality Risk  = 60% Defect Rate + 40% Non-Compliance Rate
Impact Score  = Total Spend (normalized)

Final Risk Score = 40% Delivery Risk + 30% Quality Risk + 30% Impact
Step 4 — Normalization (MinMax Scaling)
Step 5 — Excel Automation
Business Impact-
Through this analysis I got a clear data backed recommendation, Delta_Logistics should do  immediate performance review/escalation for flag, while Alpha_Inc  low-risk supplier can be considered for volume increment.

Author: Ronak Sharma

