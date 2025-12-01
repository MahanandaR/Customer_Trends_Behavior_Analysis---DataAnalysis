# Customer-trends-data-analysis-SQL-Python-PowerBI
------------------------------------------------------

## 1. Project Overview

This project examines shopping patterns and customer behavior using a dataset of 3,900 transactions across various product categories. 
The objective is to uncover insights related to spending habits, customer segmentation, product popularity, shipping behavior, and subscription preferences to support data-driven business decisions.

--------------------------------------------------------------------------------------

## 2. Dataset Summary

✤ Total Records: 3,900

✤ Features: 18

✤ Key Data Points:

✤ Customer demographics (age, gender, location, subscription status)

✤ Purchase information (product, category, purchase amount, season, color, size)

✤ Behavioral attributes (discount usage, frequency of purchases, shipping type, previous purchases)

✤ Missing Data: 37 values in the Review Rating column

--------------------------------------------------------------------------------------------------
## 3. Exploratory Data Analysis (Python)

❖ Initial analysis and preprocessing were performed using Python:

❖ Loaded and explored the dataset using pandas.

❖ Reviewed structure via .info() and descriptive statistics with .describe().

<img width="849" height="590" alt="image" src="https://github.com/user-attachments/assets/49fcbe7a-ae20-49ce-9bb4-aa1ee5921a0f" />

<img width="1390" height="620" alt="image" src="https://github.com/user-attachments/assets/1b4fdf09-8419-4695-8a0f-0d1d50071f92" />

❖ Handling Missing Data: Identified null entries and filled missing values in the Review Rating field using the median rating within each product category.

❖ Column Formatting: Standardized all column names into snake_case to improve readability and maintain consistent naming conventions.

 ❖ Feature Creation:

    • Generated an age_group variable by categorizing customers into defined age brackets.
    
    • Derived a purchase_frequency_days feature based on customer purchase intervals

❖ Data Validation: Checked the relationship between discount_applied and promo_code_used to confirm redundancy, and removed the promo_code_used column accordingly.

❖ Database Setup: Used Python to establish a connection with PostgreSQL and uploaded the transformed dataset to enable SQL-based analysis.

--------------------------------------------------------------------------------------
## 4. Data Analysis Using SQL (Business Transactions)

Conducted structured analysis in PostgreSQL to address key business questions, including:

✦ 1. Revenue by Gender – Evaluated and compared the total revenue contributed by male and female customers.

<img width="479" height="175" alt="image" src="https://github.com/user-attachments/assets/6b27c297-70e1-4ebe-afd2-6c9e883d9c05" />


✦ 2. High-Value Discount Customers – Identified customers who availed discounts yet still spent more than the overall average purchase amount.

<img width="464" height="534" alt="image" src="https://github.com/user-attachments/assets/25751088-077f-4649-afa3-e749e3d3bac4" />


✦ 3. Top 5 Products by rating - Found product with the highest average review rating.

<img width="428" height="249" alt="image" src="https://github.com/user-attachments/assets/4cdc4a29-47b7-419a-aba2-55243f0bec41" />


✦ 4. Shipping Type Comparison - Compared average purchase amounts between Standard and Express shipping methods.

<img width="371" height="156" alt="image" src="https://github.com/user-attachments/assets/77874322-f9c6-443b-b47b-f55a2b66d77a" />


✦ 5. Subscribers vs. Non-Subscribers - Evaluated differences in average spending and total revenue between subscribed and non-subscribed users.

<img width="698" height="159" alt="image" src="https://github.com/user-attachments/assets/584c7f36-67ad-414d-b2bc-7aa4f4ad393c" />


✦ 6. Discount-Dependent Products - Identified the top 5 items with the highest percentage of discounted purchases.

<img width="380" height="241" alt="image" src="https://github.com/user-attachments/assets/22ec9e0f-6eb6-42bc-b968-7f89b1547c9b" />


✦ 7.Customer Segmentation - Grouped customers into New, Returning, and Loyal categories based on their purchase frequency.

<img width="456" height="226" alt="image" src="https://github.com/user-attachments/assets/e80058d8-f2d9-4fb2-8d68-c1342b422915" />


✦ 8. Top 3 Products per Category - Extracted the three most frequently purchased products within each product category.

<img width="669" height="514" alt="image" src="https://github.com/user-attachments/assets/cb0ef7bf-800c-476b-9db7-01115f00e083" />


✦ 9. Repeat Buyers & Subscription Likelihood - Checked whether customers with over 5 purchases are more likely to subscribe to the service.

<img width="551" height="261" alt="image" src="https://github.com/user-attachments/assets/8aa19b94-c9a1-4fac-a08a-65ff8445f9d3" />


✦ 10.Revenue by Age Group - Calculated total revenue contribution across different customer age groups.

<img width="503" height="295" alt="image" src="https://github.com/user-attachments/assets/ccac31b0-aeab-4eb6-b737-277f5bf60bad" />

------------------------------------------------------------------------------------------
## 5. DashBoard
<img width="1328" height="751" alt="image" src="https://github.com/user-attachments/assets/09801922-4ac5-4cec-aca1-b84480fe6bee" />


# 👉 Dashboard Live: <a href="https://app.powerbi.com/groups/me/reports/a5f1a091-46b1-40e1-b426-6f4ff6b1ae2d/42548c50914160737db4?experience=power-bi">Click here to view the Power BI Dashboard</a>

--------------------------------------------------------
## 6. Business Recommendations

➤ Increase Subscriptions – Encourage more users to opt for subscriptions by offering exclusive perks and value-added benefits.

➤ Strengthen Customer Loyalty Programs – Provide incentives to frequent buyers to help transition them into the “Loyal” customer segment.

➤ Optimize Discount Strategy – Adjust discount levels to boost sales while maintaining healthy profit margins.

➤ Enhance Product Positioning – Promote top-rated and high-performing products more prominently in marketing campaigns.

➤ Implement Targeted Marketing – Prioritize marketing efforts toward high-value age groups and customers who prefer express shipping.
