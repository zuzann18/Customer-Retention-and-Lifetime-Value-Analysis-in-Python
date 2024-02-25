# Customer-Retention-Analysis-for-a-Telecommunication-Company
## Project Description
This project aims to build a customer retention model for a telecommunication company using historical data. The primary objective is to estimate the retention rate, average and median time to churn, and calculate the expected Customer Lifetime Value (CLV) based on three different approaches: a simple retention model, a generalized retention model, and a generalized retention model with a grouping variable.

### General Assumptions
Payments are made in arrears.
Net income from the customer is $25.
The applied discount rate is 2%.
### Methodology
Simple Retention Model
Retention Rate Estimation: Using the telco_customers.csv data, the retention rate was calculated based on the ratio of remaining customers to the total number of customers over a period.
Average Time to Churn: Calculated the average time it takes for a customer to decide to leave the service.
Median Time to Churn: Applied methodology to calculate the median time after which half of the customers have left the service.
Expected CLV Value: Calculated using a formula that considers the retention rate, net income from the customer, and the discount rate.
Generalized Retention Model
Employed the lifelines library to apply the Kaplan-Meier model to estimate the survival function of customers.
Estimated the average time to churn and the median time to churn using the survival function.
Calculated CLV for each time interval, based on the variable retention rate.
Generalized Retention Model with a Grouping Variable
Applied the Kaplan-Meier model with separate curves for different groups of customers, defined by the InternetService variable.
Compared retention rates between groups to identify which services enjoy higher customer loyalty.
### Results
Simple Retention Model: A high retention rate of 0.977 suggests that most customers remain with the company. The average time to churn is 44.15 months.
Generalized Retention Model: The median time to churn is 44 months, comparable to the simple retention model.
Generalized Retention Model with a Grouping Variable: Significant differences in retention rates depending on the type of internet service, with the highest loyalty among fiber optic users.
### Conclusions
The analysis shows that the telecommunication company has a strong position in retaining customers, especially among fiber optic internet users. Knowledge of CLV allows for better planning of marketing strategies and budgeting for acquiring new customers.

Certainly! Here's an English version for the GitHub project description:

Customer Retention Analysis for a Telecommunication Company
Project Description
This project aims to build a customer retention model for a telecommunication company using historical data. The primary objective is to estimate the retention rate, average and median time to churn, and calculate the expected Customer Lifetime Value (CLV) based on three different approaches: a simple retention model, a generalized retention model, and a generalized retention model with a grouping variable.

General Assumptions
Payments are made in arrears.
Net income from the customer is $25.
The applied discount rate is 2%.
Methodology
Simple Retention Model
Retention Rate Estimation: Using the telco_customers.csv data, the retention rate was calculated based on the ratio of remaining customers to the total number of customers over a period.
Average Time to Churn: Calculated the average time it takes for a customer to decide to leave the service.
Median Time to Churn: Applied methodology to calculate the median time after which half of the customers have left the service.
Expected CLV Value: Calculated using a formula that considers the retention rate, net income from the customer, and the discount rate.
Generalized Retention Model
Employed the lifelines library to apply the Kaplan-Meier model to estimate the survival function of customers.
Estimated the average time to churn and the median time to churn using the survival function.
Calculated CLV for each time interval, based on the variable retention rate.
Generalized Retention Model with a Grouping Variable
Applied the Kaplan-Meier model with separate curves for different groups of customers, defined by the InternetService variable.
Compared retention rates between groups to identify which services enjoy higher customer loyalty.
Results
Simple Retention Model: A high retention rate of 0.977 suggests that most customers remain with the company. The average time to churn is 44.15 months.
Generalized Retention Model: The median time to churn is 44 months, comparable to the simple retention model.
Generalized Retention Model with a Grouping Variable: Significant differences in retention rates depending on the type of internet service, with the highest loyalty among fiber optic users.
Conclusions
The analysis shows that the telecommunication company has a strong position in retaining customers, especially among fiber optic internet users. Knowledge of CLV allows for better planning of marketing strategies and budgeting for acquiring new customers.

### How to Run
To run this project, follow these steps:

Prerequisites: Ensure Python 3.6+ is installed.
Dependencies: Install required libraries via pip install pandas lifelines matplotlib.
Data: Place telco_customers.csv in the project directory.
