
# Random Forest Modeling for Employee Turnover Prediction at Salifort Motors
## Project Overview
This project developed a machine learning model to predict employee turnover for Salifort Motors. Using a dataset of 11,991 employees, we analyzed various factors including satisfaction levels, number of projects, average work hours, and other relevant features. Our Random Forest model achieved a ROC AUC score of 93.84% and an accuracy of 96.16%, providing valuable insights for HR to develop data-driven retention strategies.
## Business Understanding
Stakeholder: Salifort Motors' Human Resources Department

Business Problem: High employee turnover rates can significantly impact a company's productivity and bottom line. Salifort Motors needs to identify employees at risk of leaving and understand the key factors influencing turnover to develop effective retention strategies.

By reducing turnover, Salifort Motors can:

Minimize recruitment and training costs  
Maintain productivity and team morale  
Preserve institutional knowledge  
Enhance company reputation as an employer

## Data Understanding
The analysis utilized a dataset from Kaggle containing information on 11,991 employees. 

Key features included:  
Satisfaction level  
Number of projects  
Average monthly work hours  
Time spent at the company (tenure)  
Work accidents  
Promotions in the last 5 years  
Department  
Salary level

## Exploratory Data Analysis (EDA)

About 16.6% of employees left the company.  
Turnover rate increases as salary decreases, with over 20% of low-paid employees resigning.  
There are distinct groups of employees who left based on satisfaction levels and work hours.  
Employees handling 7 projects all left the company, indicating potential overwork.
3-4 projects seem to be the ideal workload balance.


## Modeling and Evaluation
We developed several models to predict employee turnover:

### Logistic Regression:

Accuracy: 82%  
Underperformed in predicting employees likely to leave


### Decision Tree:

ROC AUC: 95.06%  
Accuracy: 97.53%


### Random Forest:

ROC AUC: 95.64%  
Accuracy: 98.10%

### Potential Risk of Data Leakage
To address potential data leakage, we performed **feature engineering** by introducing an "overworked" column for employees working over 175 hours per month. 

Our final Random Forest model with feature engineering achieved:

ROC AUC: 93.84%  
Accuracy: 96.16%  
Precision: 87.04%  
Recall: 90.36%

### The most important features for predicting turnover:

Last evaluation score  
Number of projects  
Tenure  
Overworked status

## Conclusion
Based on our analysis, we recommend the following strategies to reduce employee turnover:

(1) Reduce Project Overload: Rebalance workloads to prevent employee burnout and boost productivity.  
(2) Implement a Recognition Program: Create rewards to motivate employees with good performance and increase their satisfaction levels.  
(3) Investigate Turnover Factors: Explore all factors beyond low satisfaction contributing to employee turnover.  
(4) Support Underperformers: Offer workshops to help employees meet project expectations and improve skills.

### Future steps to expand this project include:

Conduct regular employee surveys to gather more qualitative data on job satisfaction and work-life balance.  

Implement the model in a real-time dashboard for HR to monitor employee risk levels.  

Develop a more granular salary classification to better understand the impact of compensation on turnover.

Analyze the effectiveness of implemented retention strategies over time and adjust the model accordingly.

By implementing these recommendations and continuing to refine our predictive model, Salifort Motors can significantly improve employee retention, reducing costs and maintaining a more stable and productive workforce.