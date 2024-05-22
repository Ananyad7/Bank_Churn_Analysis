# Bank_Churn_Analysis

# Understanding Bank Customer Churn: Why Retention is Key

<img src= "https://github.com/Ananyad7/Bank_Churn_Analysis/assets/164981636/ed2cdf31-c5fb-4851-9134-f7d2d80eb797" width="2550" height="750">

Bank customer churn refers to the phenomenon where customers cease their relationship with a bank. This can manifest in several ways, such as:
Closing accounts entirely
Transferring funds to another institution
Discontinuing use of specific banking services

High customer churn acts like a silent leak in a bank's profitability. Here's why it matters:
Costly Acquisitions: Finding new customers is expensive, with marketing and onboarding surpassing the cost of retaining existing ones. Reducing churn keeps these costs in check.
Lost Revenue Streams: Churning customers take their potential future business elsewhere. Retaining them ensures a steady source of income from accounts, loans, and other services.
Damaged Reputation: A revolving door of customers suggests underlying issues. Addressing churn can rebuild trust and attract new customers seeking stability.

By tackling churn, banks can plug the leak and strengthen their financial health.

Tool used : SQL , Power BI

# About the dataset
RowNumber: Each row's unique sequential identifier.
CustomerId: A number that uniquely identifies each customer (10000).
Surname: The last name of each customer.
CreditScore: A score that reflects how financially reliable a customer is.(max:850, min:350)
Geography: Where each customer lives.(France, Spain, and Germany)
Gender: Whether the customer is male or female.
Age: How old each customer is.
Tenure: How long each customer has been with the bank (in years).
Balance: How much money each customer has in their account.
NumOfProducts: How many different bank products each customer uses.
HasCrCard: Whether each customer has a credit card (0 or 1).
IsActiveMember: Whether each customer is currently active (0 or 1).
EstimatedSalary: An estimate of each customer's annual salary.
Exited: Whether each customer has left the bank (0 or 1).

# Objective
In this report, we delve into the phenomenon of customer churn within banking institutions. Customer churn, or the rate at which customers leave a service or product, is a critical metric for banks to monitor and understand. By analyzing factors influencing churn, banks can develop strategies to retain customers and enhance customer satisfaction.
The primary objective of this report is to explore the dataset containing information about bank customers and their churn status. Through SQL analysis, we aim to identify key factors that contribute to customer churn and provide insights for mitigating churn rates.


# TUnderstanding Customer Churn Patterns in Banking Institutions

# Dataset Snapshot

<img src= "https://github.com/Ananyad7/Bank_Churn_Analysis/assets/164981636/2c3f8ed0-0e57-48f6-a761-25921992b3a5"  width="1300" height="400">


# Churn vs. Retention Rate: Total Customers
<img src= "https://github.com/Ananyad7/Bank_Churn_Analysis/assets/164981636/de42381b-e143-46ba-8978-be82d827b1a5" width="550" height="400">

Tracking churn and retention rates in banks is essential for understanding customer loyalty, improving retention strategies, and sustaining long-term growth.
The churn rate among bank customers is 20.4%, indicating that this percentage of clients have chosen to close their accounts. Conversely, the non-churn rate stands at 79.6%, reflecting the proportion of customers who have continued their banking relationship. This high retention rate underscores the satisfaction and loyalty of most of the clientele.
![image](https://github.com/Ananyad7/Bank_Churn_Analysis/assets/164981636/9fb36e23-d737-4642-a564-ce4201192e5f)


# Churn vs. Retention Rate: Location
<img src= "https://github.com/Ananyad7/Bank_Churn_Analysis/assets/164981636/725d6654-8204-430e-9e95-b499c9e6d26b" width="850" height="300">

The data reveals distinct customer dynamics across France, Spain, and Germany. France leads with 50.1% total customers, exhibiting a strong retention rate of 83.8% and a low churn rate of 16.2%. Spain follows with 24.8% customers, showing similar metrics—an 83.3% retention and a 16.7% churn rate. Germany, despite having 25.1% customers, faces significant retention challenges with a high churn rate of 32.4% and a retention rate of 67.6%. This indicates France and Spain are more effective in retaining customers compared to Germany.


# Churn vs. Retention Rate: Gender
<img src= "https://github.com/Ananyad7/Bank_Churn_Analysis/assets/164981636/0279c824-7fb9-4155-9824-5f80a0274812" width="850" height="300">

The customer distribution shows a slight skew towards males, comprising 54.6% of the total customer base, compared to 45.4% females. Notably, the churn rate is higher among female customers at 25.1%, while it stands at 16.5% for males. Consequently, male customers exhibit a higher retention rate of 83.5%, compared to 74.9% for females. This suggests that male customers are more likely to stay with the bank.


# Churn vs. Retention Rate: Age
<img src= "https://github.com/Ananyad7/Bank_Churn_Analysis/assets/164981636/41b51cc7-3732-44ae-b4e5-c138558998e1" width="850" height="300">

The customer base is skewed towards the 30-39 age group, which constitutes 43.5% of total customers and exhibits a low churn rate of 10.9%. The under 30 age group, accounting for 16.4% of customers, has the lowest churn rate at 7.6%, indicating high loyalty. Conversely, the 40-49 age group, comprising 26.2% of customers, has a significantly higher churn rate of 30.8%. The 50+ age group, representing 14.0% of the customer base, experiences the highest churn rate at 45.4%. 


# Churn vs. Retention Rate: Credit Score
<img src= "https://github.com/Ananyad7/Bank_Churn_Analysis/assets/164981636/fa923325-2de7-40ea-bf04-1e4d115678ee" width="850" height="300">

The customer base is skewed towards the Good (600-699) credit score group, which represents 38.2% of customers. Churn rates are relatively similar across groups, with the Excellent (800+) group having the lowest churn rate at 19.5%, and the Poor (300-499) group the highest at 23.7%. However, all groups maintain retention rates above 76%, with the Excellent group slightly leading at 80.5%. These findings suggest a stable customer base with minimal variance in churn rates across different credit score groups, indicating consistent satisfaction levels across credit score segments.


#  Churn vs. Retention Rate: Average Balance

<img src= "https://github.com/Ananyad7/Bank_Churn_Analysis/assets/164981636/0b52cf72-6394-4644-8f52-0acad14d3c4f" width="250" height="300">

The data reveals that churned customers have a significantly higher average account balance at $91,108.5, compared to $72,745.3 for those who have not churned. This suggests potential dissatisfaction among higher-value customers,


# Churn vs. Retention Rate: Tenure

<img src= "https://github.com/Ananyad7/Bank_Churn_Analysis/assets/164981636/13dec573-9531-46e0-a1f1-ad224edf4075" width="850" height="300">

The data indicates that newer customers have higher churn rates, with 23.0% for those with less than 1 year and 22.4% for those with 1-2 years of tenure, suggesting initial dissatisfaction. In contrast, customers with 5-10 years of tenure, who form the largest group at 50.2%, have the lowest churn rate at 19.8%, indicating greater stability and satisfaction


# Churn vs. Retention Rate: Products

<img src= "https://github.com/Ananyad7/Bank_Churn_Analysis/assets/164981636/ece4d880-46a7-44a3-9fde-d8b7409c39f5" width="850" height="300">

The data reveals clear trends in customer churn based on the number of products held. Customers with a single product show a high churn rate of 27.7%, indicating lower engagement. Conversely, those with two products have a significantly lower churn rate at 7.6%, suggesting greater satisfaction. However, churn rates soar for customers holding three or four products, reaching 82.7% and 100% respectively, pointing to potential dissatisfaction from overextension or complex product structures.



# Churn vs. Retention Rate: Credit Card

<img src= "https://github.com/Ananyad7/Bank_Churn_Analysis/assets/164981636/c4e21859-0296-4389-a9db-1df109642454" width="850" height="300">


The data reveals that both customers with and without credit cards exhibit similar churn rates around 20%, with a slightly higher churn rate among those without credit cards (20.8%) compared to those with credit cards (20.2%). This suggests that credit card status alone may not significantly influence churn behavior. 



# Churn vs. Retention Rate: Active members

<img src= "https://github.com/Ananyad7/Bank_Churn_Analysis/assets/164981636/ebdf955f-a856-4388-b59f-df0cb282abc8" width="850" height="300">


The data shows significant differences in churn rates based on membership status within the bank. Active members, comprising 51.5% of customers, exhibit a lower churn rate of 14.3%, indicating higher satisfaction and engagement. In contrast, inactive members, making up 48.5% of the customer base, have a higher churn rate of 26.9%, suggesting lower engagement and potential dissatisfaction.

# Churn vs. Retention Rate: Salary
<img src= "https://github.com/Ananyad7/Bank_Churn_Analysis/assets/164981636/da22b816-9060-48d0-8d3d-88464e04c348" width="850" height="300">


The data reveals that customers in the high salary bracket (120k+) form the largest group at 39.8% and have a slightly higher churn rate of 20.9%. Churn rates across other salary brackets are consistent, ranging from 19.1% to 20.4%. 
![image](https://github.com/Ananyad7/Bank_Churn_Analysis/assets/164981636/e62d36bc-4930-4eb5-823c-3a48f0b6b6fc)



# Recommendation

1.Develop targeted retention strategies for German customers: Implement personalized communication and engagement strategies to understand specific needs and concerns of German customers. Enhance customer support services in Germany, providing dedicated support teams to resolve issues promptly. Introduce special promotions, loyalty programs, or financial incentives to retain customers.

2.Improve Retention Among Female Customers: Focus on improving the banking experience for female customers. Create a dedicated feedback channel for female customers to voice their concerns and suggestions. Organize women-focused financial literacy programs and community events to build a stronger relationship with female customers.

3. Enhance Retention in Older Age Groups: Focus on retention strategies for customers aged 40 and above. Customized Products: Develop financial products that cater to the needs of customers in the 40-49 and 50+ age groups, such as retirement planning services.
 
4. Engage High-Value Customers: Pay special attention to customers with higher account balances. Provide VIP services or dedicated account managers for high-value customers to enhance their banking experience.
Offer exclusive benefits, such as higher interest rates on savings or lower loan rates, to high-value customers.
6. Optimize Product Offerings: Simplify and optimize product offerings. Conduct a review of current products to identify and eliminate those that may be causing customer dissatisfaction. Use customer feedback to continuously refine and improve product offerings.
7. Strengthen Engagement with Inactive Members: Develop strategies to re-engage inactive members. Launch targeted re-engagement campaigns offering incentives for inactive members to become active again.
Implement activity monitoring to identify signs of inactivity early and intervene with personalized offers or support.
8. Leverage Credit Card Usage Insights: Promote credit card usage as part of a broader customer engagement strategy. Introduce incentive programs that reward customers for using their credit cards, such as cashback offers or reward points. Provide education on the benefits and responsible use of credit cards to help customers see the value in maintaining a credit card. Create bundled offers that combine credit cards with other bank products to increase overall engagement and satisfaction.
9. Maintain High Service Standards for High-Salary Bracket: Ensure high service standards for customers in the high-salary bracket. Offer tailored financial advice and investment opportunities for high-salary customers. Provide exclusive banking services, such as priority customer service and access to premium banking products.

By implementing these recommendations, the bank can address the specific factors contributing to customer churn and work towards improving overall customer retention.





