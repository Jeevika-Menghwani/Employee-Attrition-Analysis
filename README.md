# 🏢 Employee Attrition Analysis: Data-Driven Insights

📌 Overview

This project applies exploratory data analysis (EDA), machine learning, and model evaluation techniques to predict employee attrition and uncover key drivers behind turnover. The insights derived can help HR teams implement proactive retention strategies.

📊 Dataset

Size: 1470 observations, 13 features
Key Features:
Numerical: Age, Monthly Income, Distance from Home
Categorical: Department, Marital Status, Job Satisfaction
Data Integrity: No missing values
⚠️ Class Imbalance Challenge

Attrition Distribution: 83.9% (No) vs. 16.1% (Yes)
Impact on Modeling: Required SMOTE (Synthetic Minority Oversampling Technique) to balance classes and improve minority class predictions.
📈 Exploratory Data Analysis (EDA)

Age: Employees who left had a mean age of 33.6 vs. 37.5 for those who stayed.
Distance from Home: Higher attrition risk for employees living farther (10.6 miles) vs. those closer (8.9 miles).
Monthly Income: Lower salaries correlated with higher attrition ($4787 vs. $6832).
🤖 Machine Learning Models

1️⃣ Logistic Regression
Key Features Identified:
✅ Age (Younger employees leave more)
✅ Monthly Income (Higher salaries reduce attrition)
✅ Distance from Home (Farther distance increases attrition risk)
✅ Job Satisfaction & Work-Life Balance (Higher satisfaction lowers attrition)
✅ Marital Status (Single employees are more likely to leave)
Model Performance:
Training Accuracy: 84.13%
Test Accuracy: 83.50%
Issue: Poor sensitivity (unable to detect attrition cases effectively).
2️⃣ Random Forest Classifier
Hyperparameter Optimization: Conducted using GridSearchCV
Performance:
Training Accuracy: 86.62%
Test Accuracy: 84.35%
Key Takeaway:
Performs well on majority class but struggles with minority class (attrition cases).
Balanced Accuracy: 52.99% (slightly better than random guessing).
📊 Key Findings & Business Impact

Attrition Drivers Identified: HR can focus on improving salaries, job satisfaction, and work-life balance.
Retention Strategies: Predictive insights enable targeted interventions such as compensation adjustments and career growth opportunities.
Model Limitation: Addressing class imbalance through resampling techniques or alternative algorithms can improve minority class predictions.
