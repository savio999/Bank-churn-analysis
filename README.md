# Bank-churn-analysis

Dataset is taken from https://www.kaggle.com/datasets/radheshyamkollipara/bank-customer-churn

About Dataset
RowNumber—corresponds to the record (row) number and has no effect on the output.
CustomerId—contains random values and has no effect on customer leaving the bank.
Surname—the surname of a customer has no impact on their decision to leave the bank.
CreditScore—can have an effect on customer churn, since a customer with a higher credit score is less likely to leave the bank.
Geography—a customer’s location can affect their decision to leave the bank.
Gender—it’s interesting to explore whether gender plays a role in a customer leaving the bank.
Age—this is certainly relevant, since older customers are less likely to leave their bank than younger ones.
Tenure—refers to the number of years that the customer has been a client of the bank. Normally, older clients are more loyal and less likely to leave a bank.
Balance—also a very good indicator of customer churn, as people with a higher balance in their accounts are less likely to leave the bank compared to those with lower balances.
NumOfProducts—refers to the number of products that a customer has purchased through the bank.
HasCrCard—denotes whether or not a customer has a credit card. This column is also relevant, since people with a credit card are less likely to leave the bank.
IsActiveMember—active customers are less likely to leave the bank.
EstimatedSalary—as with balance, people with lower salaries are more likely to leave the bank compared to those with higher salaries.
Exited—whether or not the customer left the bank.
Complain—customer has complaint or not.
Satisfaction Score—Score provided by the customer for their complaint resolution.
Card Type—type of card hold by the customer.
Points Earned—the points earned by the customer for using credit card.
Objective
As we know, it is much more expensive to sign in a new client than keeping an existing one. It is advantageous for banks to know what leads a client towards the decision to leave the company. Churn prevention allows companies to develop loyalty programs and retention campaigns to keep as many customers as possible.
 
Data cleaning and modelling

•	The dataset contains 10,000 rows.
•	Upon inspection, no data errors or inconsistencies were found.
•	Data types for all columns were verified and found to be appropriate.
•	The “RowNumber” column was removed as it was not relevant for analysis.
•	No duplicate records were detected in the dataset.

Relation View
 

From the main fact table “Customer-Churn-Records”, the following dimension tables were created to enhance reporting and analysis:
1.	Credit Card Holders
2.	Geography
3.	Gender
4.	Active Members
5.	Exited
All the above tables maintain a one-to-many relationship with the fact table (Customer-Churn-Records), enabling efficient data modeling and improved report performance.



Reports

I have created reports in 3 pages:

1. Overview:

 

Dataset Overview and Key Insights:
•	The dataset contains 10,000 customer records, with an overall churn rate of 20.4%.
•	A total of 2,044 complaints were received, and the average customer satisfaction score is 3.01 out of 5.
•	7,055 customers hold credit cards.
•	The bank has 5,151 active and 4,849 inactive members. Inactive customers show a higher churn rate (25.87%) compared to active members (14.27%).
Demographic Insights:
•	Customers are grouped by age as 1–18, 19–25, 26–35, 36–59, and 60+ years.
•	Minor accounts (1–18 years) have the churn rate of (9.09%).
•	Churn increases with age, peaking at 29.02% in the 36–59 age group, while senior citizens (60+) have the second-highest churn rate (27.95%).
Financial Insights:
•	Customers are categorized by bank balance into <50K, 50K–100K, 100K–200K, and 200K+ groups.
•	The churn rate increases progressively with higher balances — 25.02% for 100K–200K and 55.08% for 200K+ customers, indicating that high-balance customers are more likely to churn.

2. Churn Breakdown:

 

a. Based on the Tenure chart (grouped into 0–2, 3–6, 7–9, and 10+ years), the churn rate increases from the 0–2 group to the 3–6 group, and then gradually decreases thereafter. Customers with a tenure of 10 years or more show the lowest churn rate.
b. The churn rate is higher among females (55%) compared to males (44%).
c. Among countries, France records the highest churn, followed by Germany, while Spain has the lowest churn rate.
d. Customers with higher credit scores and a greater number of products tend to have lower churn rates.
e.  A total of 685 customers with credit scores between 580–669 churned, making this range the most affected segment.
f. Interestingly, customers with an estimated salary between 100K–200K show the highest churn, with 1,045 customers leaving.

3. Credit Card Churn:  

Customers without credit cards show a slightly higher churn rate compared to those who have credit cards. However, there is not much variation in churn among different credit card holders — the difference is around 20% or less.

Conclusion
The analysis of the Customer Churn dataset (10,000 records) provides valuable insights into customer behavior and the key factors influencing churn.
The overall churn rate is 20.4%, with higher churn observed among females, inactive members, and customers with higher account balances. France records the highest churn, while Spain performs the best in customer retention.
Tenure analysis reveals that customers with shorter relationships (3–6 years) are more likely to churn, whereas those with 10+ years of association show the highest loyalty. Similarly, customers with higher credit scores and multiple products demonstrate lower churn tendencies.
Interestingly, customers earning between 100K–200K show the highest churn, suggesting that income alone does not guarantee loyalty.


