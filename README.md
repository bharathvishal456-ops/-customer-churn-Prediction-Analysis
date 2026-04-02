Customer Churn Prediction Analysis
Project Overview
This project focuses on analyzing a synthetic customer dataset to identify key factors contributing to customer churn. Through a series of data generation, cleaning, statistical analysis, and visualization steps, we aim to understand customer behavior and provide actionable insights for retention strategies.

Project Steps & Analysis
1. Data Generation
Methodology: A synthetic dataset of 100,000 customer records was generated using Faker and NumPy to simulate various customer attributes. pandas was used to create a DataFrame from this data.
Attributes: The dataset includes Customer_ID, Age, Gender, Tenure, Balance, CreditScore, EstimatedSalary, NumOfProducts, IsActiveMember, and Churn.
Output: The generated data was saved as customer_data.csv and loaded into a pandas DataFrame named df.
2. Data Cleaning & Preprocessing
Missing Values: Checked for any missing values across all columns. The synthetic data was found to be clean with no missing values.
Data Types: Verified data types for all columns to ensure they are appropriate for analysis.
3. Descriptive Statistics
Numerical Features: Calculated mean, median, mode, and standard deviation for numerical columns (Age, Tenure, Balance, CreditScore, EstimatedSalary, NumOfProducts).
Categorical Features: Examined descriptive statistics, including mode, for categorical columns (Gender, IsActiveMember, Churn).
4. Churn Behavior Analysis
Overall Churn Distribution: Visualized the percentage of churned vs. non-churned customers using a bar plot.
Categorical Feature Comparison: Explored churn rates across different categories using count plots:
Churn by Gender
Churn by Active Member Status (IsActiveMember)
Churn by Number of Products (NumOfProducts)
Numerical Feature Comparison: Compared the distribution of key numerical features for churned vs. non-churned customers using box plots:
Age vs. Churn
Tenure vs. Churn
Balance vs. Churn
CreditScore vs. Churn
EstimatedSalary vs. Churn
5. Group-Based Analysis
Age Group vs. Churn: Created age bins and calculated the churn rate for each age group, visualizing the findings with a bar plot. This revealed that customers in the 25-54 age range tend to have higher churn rates.
6. Relationship Analysis
Balance vs. Estimated Salary by Churn: A scatter plot was generated to visualize the relationship between customer Balance and EstimatedSalary, with points colored by their Churn status.
Correlation Matrix: A heatmap displayed the correlation matrix for all numerical features, including Churn, to identify linear relationships between variables.
7. Data Visualization (Further Explorations)
Gender Distribution: A pie chart illustrated the proportional distribution of Male and Female customers.
Age Distribution: A histogram with a KDE plot showed the overall distribution of customer Age.
Key Insights & Conclusion
Based on the analysis, several factors were identified as potential drivers of customer churn:

Age: Customers in the 25-54 age groups exhibit a higher propensity to churn.
Active Membership: Inactive members are significantly more likely to churn compared to active members.
Number of Products: Customers holding 3 or 4 products show a much higher churn rate, suggesting potential dissatisfaction or complexity with multiple services.
Balance & Credit Score: Churned customers tend to have slightly lower average balances and credit scores, although the difference is not extremely pronounced.
Tenure: Customers with lower tenure (newer customers) might be at a slightly higher risk of churning.
Proposed Business Improvements
To mitigate customer churn, the following strategies could be considered:

Targeted Retention Programs: Develop specific retention campaigns for customers in the high-risk age groups (25-54) and for those who become inactive.
Re-engagement Strategies: Implement proactive re-engagement efforts for customers showing signs of inactivity, possibly offering personalized incentives.
Product Optimization: Investigate the reasons behind high churn rates among customers with multiple products. This could involve simplifying product offerings, improving customer support for multi-product users, or ensuring the value proposition is clear.
Financial Well-being Support: Offer financial literacy resources or personalized advice for customers with lower balances or credit scores, which could indirectly improve their satisfaction and reduce churn.
New Customer Nurturing: Focus on enhanced onboarding and support for new customers (lower tenure) to build stronger loyalty early on.
By addressing these key areas, the business can aim to reduce churn and improve overall customer lifetime value.
