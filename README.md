# European-Bank-Churn-Analysis

##  Project Overview
This project aims to perform a comprehensive churn analysis for a European bank using customer data across France, Germany, and Spain. The goal is to explore customer behavior, identify patterns that contribute to customer churn, and generate actionable insights that can help improve retention strategies.

I plan to analyze a dataset of 10,000 bank customers, focusing on demographic factors (age, gender, country), financial indicators (account balance, estimated salary), and account behaviors (credit card ownership, active status). The final output will include visual dashboards that break down churn distribution across key segments.

## Problem Statement
In today’s competitive banking landscape, customer retention is a critical factor in sustaining profitability and growth. European banks face increasing challenges due to customer churn, which can lead to substantial revenue loss and decreased customer lifetime value.

This project is focused on analyzing customer data from a European bank to uncover the factors contributing to churn. By understanding demographic and behavioral patterns, the bank can implement targeted strategies to improve customer loyalty and retention.

##  Key Questions Answered by the Analysis
1. What is the overall churn rate across the bank's customer base?

2. How is customer distribution spread across different countries (France, Germany, Spain)?

3. Which age group contains the most customers, and how does churn vary across age groups?

4. What is the gender distribution among customers, and does it relate to churn?

5. How many customers own credit cards, and how does this relate to churn behavior?

6. How does account balance influence the likelihood of a customer churning?

7. Which country has the highest churn rate, and what does customer behavior look like in each country?

## Data Source
The dataset used in this analysis reflects real-world banking records and was sourced from Maven Analytics. It contains detailed information on 10,000 customers from a European bank, covering demographics, account features, financial activity, and churn status.

To ensure customer privacy, all personally identifiable information (PII) has been removed. Where applicable, synthetic values were generated to replace sensitive data while preserving the natural patterns of customer behavior and churn. This approach maintains the dataset’s integrity and makes it suitable for meaningful business analysis and predictive modeling.

## Tools Used
### Power Bi
**Power Query:** For data cleaning and transformation

**DAX:** Used to create calculation measures and perform advanced analytics

**Charts & Visuals:** Built interactive dashboards using bar, column, donut, matrix, and Tree map

## Data Analysis Process
**Data Cleaning & Transformation:** The process began with handling missing values, transforming numerical codes into meaningful text labels, and creating conditional columns to categorize data into ranges—making patterns easier to interpret and analyze.

**Exploratory Data Analysis (EDA):** Analyzed churn trends in relation to key variables including country, age group, account balance, gender, and credit card ownership status.

**DAX Calculations:** Data Analysis Expressions (DAX) was used to create custom measures and KPIs, including:
```DAX
Total Customers = COUNT(Bank_Churn[CustomerId])
Churn Rate = Bank_Churn[Churn Count]/ [Total Customers]
Avg Estimated Salary = AVERAGE(Bank_Churn[EstimatedSalary])
Avg Credit Score = AVERAGE(Bank_Churn[CreditScore])
```

## European Bank Churn Analysis Dashboards Showing Insights
![Screenshot 2025-05-16 044256](https://github.com/user-attachments/assets/6e72bf8d-4ee4-4451-a6d2-e48ea6135d42)
![Screenshot 2025-05-16 044220](https://github.com/user-attachments/assets/affbbdfc-b4ca-46df-a59d-3e02a88feab0)

## Insight Deep Dive
1. **Churn Rate by Age Group**
- **Insight:** The age group 51–60 has the highest churn rate at 56.2%, followed by 41–50 (34%) and 61–70 (31.4%).

- **Business Implication:** Customers in their mid to late career or early retirement stage may feel neglected or overwhelmed by modern banking tools. There’s a need to improve digital literacy support, simplify mobile interfaces, or provide concierge-style customer service for this age range.

2. **Churn Rate by Country**
- **Insight:** Germany records the highest churn rate at 32.4%, compared to Spain (16.7%) and France (16.2%).

- **Business Implication:** The German market may be experiencing service dissatisfaction or aggressive competitor poaching. The bank should run market-specific diagnostics—customer feedback, competitor benchmarking—and potentially deploy a localized churn reduction initiative.

3. **Churn Rate by Account Balance**
- **Insight:** Customers with ₦1k–₦10k and those with balances above ₦200k have the highest churn rates at 100% and 55.9%, respectively.

- **Business Implication:** Low-balance customers likely churn due to financial pressure or limited perceived value. Offer financial wellness tools or small incentive programs.

     - High-balance customers might be lured by premium competitors. Introduce loyalty tiers or exclusive services to retain these high-value clients.

4. **Churn Rate by Product Quantity**
- **Insight:** Customers holding 3 or 4 products experience the highest churn rates at 82.7% and 100% respectively.

- **Business Implication:** This indicates a lack of perceived value in bundled offerings. Investigate if customers feel forced into packages or can’t fully utilize them. Redesign modular, need-based bundles that promote usage and satisfaction rather than quantity.

5. **Churn Rate by Activity Status**
- **Insight:** Inactive customers have a churn rate of 26.9%, nearly double that of active users (14.3%).

- **Business Implication:** Lack of regular engagement is a strong churn predictor. Build targeted reactivation campaigns, like gamified check-ins, push notifications, and exclusive return offers, to re-engage these users.

6. **Churn Rate by Gender**
- **Insight:** Female customers have a churn rate of 25.1%, higher than males at 16.5%.

- **Business Implication:** This suggests that current services may not resonate equally across genders. Conduct gender-sensitive surveys or listening sessions, and introduce financial tools tailored for women (e.g., investment education, maternity savings plans, etc.).

7. **Churn Rate by Credit Card Status**
- **Insight:** Churn rates for customers with and without credit cards are similar (Owned: 20.2%, Not Owned: 20.8%).

- **Business Implication:** Credit card ownership alone doesn’t influence retention. Consider bundling cards with cashback, rewards, or bill management tools to increase value and stickiness.

8. **Credit Score by Churn Status**
- **Insight:** Customers who churn have lower average credit scores compared to retained customers.

- **Business Implication:** This group is more likely to face financial stress and disengage due to debt or low confidence. Offer preventive credit management resources—alerts, tips, or temporary relief programs—to reduce attrition among financially vulnerable customers.

## Recommendation 
1. **Churn Rate by Age Group (51–60 years at 56.2%)**

**Recommendation:**
Introduce a customer retention program specifically for mid-to-late age customers (51–70). This can include simplified digital interfaces, personalized customer support, and financial planning tools tailored to retirement preparation. Consider assigning relationship managers for personalized engagement.

2. **Churn Rate by Country (Germany at 32.4%)**

**Recommendation:**
Conduct a comprehensive root cause analysis in the German market, including NPS surveys and churn interviews. Based on findings, implement localized service improvements, such as more responsive customer care or competitive product pricing. Deploy region-specific marketing campaigns to rebuild trust and engagement.

3. **Churn Rate by Account Balance (₦1k–₦10k and >₦200k are highest)**

**Recommendation:**
Segment customers by account balance and develop tiered retention strategies:

For low-balance customers: Introduce micro-incentives, no-fee digital services, and budget management tools.

For high-balance customers: Launch a “Premier Customer Program” offering wealth advisory, dedicated support, and exclusive investment opportunities.

4. **Churn Rate by Product Quantity (High churn at 3–4 products)**

**Recommendation:**
Reevaluate bundled product offerings to ensure they are value-driven, not volume-driven. Use behavioral analytics to understand which products are underutilized or confusing. Shift to modular product packaging that allows users to select only the services they need, and accompany new bundles with onboarding guidance.

5. **Churn Rate by Activity Status (Inactive: 26.9%, Active: 14.3%)**

**Recommendation:**
Implement a customer activity monitoring system to flag inactive users early. Use this to trigger personalized re-engagement workflows — such as in-app messages, email nudges, and loyalty offers — that encourage renewed activity before customers churn completely.

6. **Churn Rate by Gender (Female: 25.1%, Male: 16.5%)**

**Recommendation:**
Launch a targeted gender-based customer experience audit to identify pain points among female users. Develop and promote products designed around women’s financial journeys, and ensure inclusive communication and representation across all customer touchpoints.

7. **Churn Rate by Credit Card Ownership (No significant impact)**

**Recommendation:**
Refocus credit card campaigns from acquisition to value enhancement. Integrate cards into broader financial wellness programs, such as cashback rewards, financial tracking tools, or exclusive partnerships that drive loyalty and long-term engagement.

8. **Credit Score by Churn Status (Lower among churned customers)**

**Recommendation:**
Create a proactive credit health monitoring initiative that uses score changes as early churn indicators. Offer automated nudges, financial advice, or short-term credit relief to support at-risk customers and maintain trust before disengagement occurs.














