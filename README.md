
# **Customer Retention Analysis for a Telecommunication Company**  
### **Kaplan-Meier Model Implementation for Customer Churn Prediction**

## **Project Overview**  
This project applies **Kaplan-Meier survival analysis** to estimate customer retention rates and predict churn for a telecommunication company. By analyzing historical data, we aim to quantify retention trends and calculate **Customer Lifetime Value (CLV)** using three different modeling approaches:  

1. **Simple Retention Model** – A basic estimation of retention rates and churn times.  
2. **Generalized Retention Model** – Advanced survival analysis using the **lifelines** library.  
3. **Generalized Retention Model with Grouping** – Segmentation by **Internet Service type** to compare customer loyalty across groups.  

## **Key Assumptions**  
- Payments are made in arrears.  
- The average net income per customer is **$25** per period.  
- A **2% discount rate** is applied for CLV calculations.  

## **Methodology**  

### **1. Simple Retention Model**  
- **Retention Rate**: Calculated as the ratio of active customers over time.  
- **Time to Churn**: Average and median time before customer departure.  
- **Expected CLV**: Derived using retention rate, net income, and discount rate.  

### **2. Generalized Retention Model**  
- Utilizes the **Kaplan-Meier survival function** to estimate churn probability.  
- Computes **average and median churn times** using survival analysis.  
- Predicts CLV dynamically by accounting for a variable retention rate.  

### **3. Generalized Retention Model with Grouping**  
- Applies the **Kaplan-Meier model** to different customer groups (e.g., Fiber Optic vs. DSL users).  
- Identifies differences in **customer loyalty** based on service type.  

## **Data Preparation**  
The dataset (`telco_customers.csv`) includes essential features for retention analysis:  
- **tenure**: Customer’s service duration (in months).  
- **cancel**: Churn indicator (1 = churned, 0 = active).  

Data is **sorted by tenure** to align with the sequential nature of survival analysis.  

## **Key Findings**  

- **High Retention Rate (0.977)**: Most customers stay with the company.  
- **Median Time to Churn (44 months)**: Customers typically leave after nearly 4 years.  
- **Service-Based Loyalty**: Fiber Optic users exhibit higher retention rates.  

## **Conclusion**  
The telecommunication company demonstrates **strong customer retention**, particularly among **fiber optic users**. Insights from this analysis enable **strategic marketing decisions** and better budgeting for customer acquisition.  

## **How to Run the Project**  

### **Prerequisites**  
- Python **3.6+**  
- Required libraries:  
  ```bash
  pip install pandas lifelines matplotlib
  ```
- Place `telco_customers.csv` in the project directory.  

### **Execution**  
Run the Jupyter Notebook or Python script to generate retention insights and visualize Kaplan-Meier survival curves.  

