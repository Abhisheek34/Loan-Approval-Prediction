# Loan Approval Prediction Using Machine Learning

📌 Project Overview
This project predicts whether a loan application will be approved or rejected based on customer details. It uses machine learning algorithms to analyze financial history, credit scores, income, and loan details.

🚀 **Project Summary**
Dataset: 45,000 records with 14 features
Target Variable: loan_status (1 = Approved, 0 = Rejected)

Techniques Used:
Feature Engineering: Standardization, correlation analysis, VIF check
Handling Imbalanced Data: Used SMOTE to balance loan_status
Machine Learning Models:
Logistic Regression (AUC: 96%) ✅
Decision Tree (AUC: 86%)
Random Forest, SVM, KNN, Gradient Boosting, Adaboost

**Dataset Details**

person_age (Float): Age of the person  
person_gender (Categorical): Gender of the person    
person_education (Categorical): Highest education level  
person_income (Float): Annual income  
person_emp_exp (Integer): Years of employment experience  
person_home_ownership (Categorical): Home ownership status (e.g., rent, own, mortgage)  
loan_amnt (Float): Loan amount requested  
loan_intent (Float): Purpose of the loan  
loan_int_rate (Float): Loan interest rate  
loan_percent_income (Float): Loan amount as a percentage of annual income  
cb_person_cred_hist_length (Float): Length of credit history in years  
credit_score (Integer): Credit score of the person  
previous_loan_defaults_on_file (Categorical): Indicator of previous loan defaults  
loan_status : Loan approval status (Integer): 1 = approved; 0 = rejected  

**Model Performance Comparison**

| Model                  | Train Accuracy | Test Accuracy | AUC Score |
|------------------------|---------------|--------------|-----------|
| Logistic Regression    | 90%           | 90%          | 96%       |
| K-Nearest Neighbors   | 99%           | 93%          | 93%       |
| Support Vector Machine | 91%           | 90%          | 90%       |
| Decision Tree         | 93%           | 92%          | 86%       |
| Random Forest        | 100%          | 93%          | 87%       |
| AdaBoost             | 90%           | 90%          | 84%       |
| Gradient Boost      | 93%           | 92%          | 88%       |

**✨ Key Insights**

✅ Logistic Regression is the best model with 96% AUC after balancing data using SMOTE.  
✅ Random Forest & Decision Tree are prone to overfitting (high train accuracy but lower test AUC).  
✅ SMOTE improved model performance by balancing class distribution.  
