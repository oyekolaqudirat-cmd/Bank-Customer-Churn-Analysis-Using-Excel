# Bank Customer Churn Analysis Using Excel
### 1. Project Overview

Customer retention is an important concern for financial institutions because losing existing customers can affect revenue, customer lifetime value, and long-term business growth. This project analyses a bank customer dataset to identify patterns associated with customer churn. Microsoft Excel was used for data preparation, feature engineering, analysis, PivotTables, and visualization.
The analysis focuses on understanding which customer characteristics and banking behaviors are associated with higher or lower churn rates.

### 2. Business Objective

The primary objective of this project is to analyse customer churn and identify customer segments with different levels.
- Determine the overall customer churn rate.
- Analyse churn patterns across customer demographics.
- Examine churn across different geographical locations.
- Investigate the relationship between customer activity and churn.
- Analyse how the number of banking products relates to customer churn.
- Examine the relationship between account balance and churn.
- Investigate whether customer tenure is associated with different churn rates.
- Identify customer segments that may require further retention analysis.

### 3. Dataset Overview

The dataset contains 10,000 customer records and information relating to customer demographics, banking behaviour, and churn status.

| Column | Description |
|---|---|
| Customer ID | Unique identifier assigned to each customer |
| Geography | Country where the customer is located |
| Credit Score | Credit score of the customer |
| Age | Age of the customer |
| Gender | Gender of the customer |
| Tenure | Number of years the customer has stayed with the bank |
| Balance | Customer's account balance |
| Number of Products | Number of banking products used by the customer |
| Has Credit Card | Indicates whether the customer has a credit card |
| Is Active Member | Indicates whether the customer is an active member of the bank |
| Estimated Salary | Estimated salary of the customer |
| Exited | Indicates whether the customer has left the bank |

### 4. Data Preparation

Before analysis, the dataset was reviewed and prepared for analysis in Microsoft Excel.
The preparation process included:
- Checking the dataset structure.
- Reviewing data types.
- Checking for missing values.
- Checking for duplicate records.
- Verifying categorical values.
- Checking numerical fields for inconsistencies.
- Preparing the dataset for PivotTable analysis.
  
The original dataset was preserved, while additional calculated columns were created for analysis.

### 5. Feature Engineering

Feature engineering was performed to transform existing variables into categories that would make customer segments easier to analyze.

**5.1 Age Group**

Purpose: To compare churn rates across different age groups.

Customers were grouped into age ranges: 
-	18–35
-	36-64
-	65-79
-	80+

**5.2 Tenure Group**

Purpose: To investigate whether the length of the customer relationship is associated with churn.

Customer tenure was grouped into:
-	0–2 Years
- 3–5 Years
-	6–8 Years
-	9–10 Years
  

**5.3 Credit Score Category**

Credit scores were grouped into categories such as:
-	Low
-	Good
-	Fair
-	Excellent

Purpose: To make it easier to compare churn across different credit-score groups.

**5.4 Balance Category**

Customers were divided into:
- Zero Balance
-	Positive Balance
  
Purpose: To compare churn behaviour between customers with and without a positive account balance.

**5.5 Product Category**

Customers were grouped according to the number of banking products they use.
-	Single Product
-	Two Product
-	Three Product
-	Four Product

 	Purpose: To examine whether product usage is associated with customer churn.

### 6.  Analysis

The analysis was performed using Excel PivotTables, calculated metrics, and charts.

The following areas were investigated:
- Customer Churn: Total customers, Churned customers, Retained customers, Overall churn rate.
- Customer Demographics: Age, Age group, Gender, Geography.
- Customer Behaviour: Active vs inactive members, Number of products, Credit card ownership, Account balance.
- Customer Relationship: Customer tenure, Tenure groups

### 7. Key Performance Indicators

The main KPIs used in the analysis were:

| KPI | Description | Overall Results |
|---|---|---:|
| Total Customers | Total number of customers in the dataset | 10,000 |
| Churned Customers | Number of customers who left the bank | 2,037 |
| Retained Customers | Number of customers who remained with the bank | 7,963 |
| Churn Rate | Percentage of customers who exited the bank | 20.37% |
| Retention Rate | Percentage of customers who remained with the bank | 79.63% |

### 8. Customer Churn Analysis

**8.1 Churn by Geography**

| Geography | Customers | Churn Rate |
|---|---:|---:|
| Germany | 2,509 | 32.44% |
| Spain | 2,477 | 16.67% |
| France | 5,014 | 16.15% |

Interpretation:
Germany recorded the highest observed churn rate among the three countries, while France recorded the lowest. This indicates that churn varies geographically within the dataset. 

**8.2 Churn by Customer Activity**

| Activity Status | Customers | Churn Rate |
|---|---:|---:|
| Inactive | 4,849 | 26.85% |
| Active | 5,151 | 14.27% |

Interpretation:
Inactive customers recorded a higher churn rate than active customers.

This suggests an association between customer activity and churn. Customer engagement could therefore be an area for the bank to investigate when developing retention strategies.

**8.3 Churn by Age Group**

| Age Group | Customers | Churn Rate |
|---|---:|---:|
| 18–29 | 1,641 | 7.56% |
| 30–39 | 4,346 | 10.88% |
| 40–49 | 2,618 | 30.79% |
| 50–59 | 869 | 56.04% |
| 60+ | 526 | 27.95% |

Interpretation:
The 50–59 age group recorded the highest observed churn rate, while customers aged 18–29 recorded the lowest.

The result suggests that churn varies considerably across age groups. Further analysis could investigate whether differences in banking needs, product usage, or customer engagement are associated with these differences.

**8.4 Churn by Number of Products**

| Number of Products | Customers | Churn Rate |
|---|---:|---:|
| 1 | 5,084 | 27.71% |
| 2 | 4,590 | 7.58% |
| 3 | 266 | 82.71% |
| 4 | 60 | 100.00% |

Interpretation:
Customers using three or four products recorded substantially higher observed churn rates.

However, the number of customers using three or four products is relatively small compared with customers using one or two products. Therefore, these results should be interpreted cautiously.

The bank could investigate whether these customers experienced specific product-related issues or whether the small sample sizes are influencing the observed rates.

**8.5 Churn by Account Balance**

| Balance Category | Customers | Churn Rate |
|---|---:|---:|
| Zero Balance | 3,617 | 13.82% |
| Positive Balance | 6,383 | 24.08% |

Interpretation:
Customers with positive account balances recorded a higher observed churn rate than customers with zero balances.

This pattern could be explored further by examining balance ranges, customer activity, product usage, and other customer characteristics.

### 9. Dashboard
An Excel dashboard was created to present the major findings in an interactive and easy-to-understand format.

Dashboard Components

***KPI Cards***
-	Total Customers
-	Churned Customers
-	Retained Customers
-	Churn Rate
-	Retention Rate
  
***Charts***
-	Churn by Geography
-	Churn by Age Group
-	Churn by Activity Status (Active Members)
-	Churn by Product Category
-	Churn by Balance Category
-	Churn by Credit score
  
***Slicers***
-	Geography 
-	Age Group 
-	Product Category 
-	Credit Score Category
  
![Image of dashboard](https://github.com/oyekolaqudirat-cmd/Bank-Customer-Churn-Analysis-Using-Excel/blob/main/Bank%20churn%20Dashdoard.png)

### 10. Key Insights

The analysis identified several notable patterns:
- The overall customer churn rate was 20.37%.
- Germany recorded the highest observed churn rate among the three countries.
- Inactive customers had a higher churn rate than active customers.
- Churn varied substantially across age groups, with the 36-64 group recording the highest observed rate.
- Customers using three or four products had particularly high observed churn rates, although these groups contain relatively few customers.
- Customers with positive account balances had a higher observed churn rate than customers with zero balances.

### 11. Business Recommendations

Based on the observed patterns, the bank could consider:
- Investigating inactive customers
  
Analyze why inactive customers are leaving and explore customer engagement initiatives that encourage continued interaction with banking services.
- Investigating geographical differences
  
Further examine customer experience, service delivery, and product usage across countries, particularly where churn rates differ substantially.
- Understanding age-related churn
  
Investigate whether customers in higher-churn age groups have different banking needs or service expectations.
- Reviewing product-related churn
  
Customers using multiple products should be investigated further to understand whether product complexity, suitability, or service issues are associated with their higher observed churn.

### 12. Limitations

This analysis identifies patterns and associations, not causal relationships.
The dataset does not provide information such as:
- Reasons customers left the bank
-	Customer satisfaction scores
-	Customer complaints
-	Detailed transaction history
-	Customer service interactions
-	Reasons for opening or closing products
  
Therefore, the observed relationships cannot by themselves establish why a customer churned.

Some segments, particularly customers using three or four products, also contain relatively few observations, so their churn rates should be interpreted cautiously.

### 13. Tools Used / Data Source
Microsoft Excel: Data Cleaning, Feature Engineering, Excel Formulas, PivotTables, Pivot Charts, Data Visualization, Dashboard Development

The data is from maven analytics data playground
[Click here](https://mavenanalytics.io/data-playground/bank-customer-churn)

### 14. Conclusion

This project analyzed 10,000 bank customer records to investigate customer churn patterns using Microsoft Excel.
The analysis found an overall churn rate of 20.37% and identified differences in churn across geography, age groups, customer activity, product usage, and account balance.

The findings provide a basis for further investigation into customer retention. In particular, differences in customer activity, geographical location, age, and product usage could be explored alongside additional customer information to better understand the factors associated with churn.

Overall, the project demonstrates how Excel can be used to transform raw customer data into structured business insights that support data-driven customer retention analysis.

