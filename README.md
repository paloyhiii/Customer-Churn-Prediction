# Telecom Customer Churn Prediction

## Project Overview
This project aims to predict customer churn in the telecommunications industry using machine learning techniques. The objective is to identify customers with a high likelihood of churn in order to support proactive retention strategies.

## Business Context
Customer acquisition in the telecom sector is significantly more costly than customer retention. By analyzing customer demographics, service usage, and contract characteristics, this project provides insights to help businesses reduce churn and improve long-term customer value.

## Dataset
The analysis uses the public Telco Customer Churn dataset, consisting of 7,043 customer records with 21 features.

- Features include customer demographics, subscribed services, contract type, tenure, and billing information.
- Target variable: `Churn` (Yes / No).

## Methodology

### Exploratory Data Analysis (EDA)
- Conducted univariate and bivariate analysis to explore churn patterns.
- Identified key churn drivers such as contract type, tenure, and monthly charges.

### Data Preprocessing
- Handled missing values in numerical variables.
- Applied label encoding and one-hot encoding to categorical features.
- Addressed class imbalance to improve model sensitivity toward churned customers.

### Modeling & Optimization
- Trained and evaluated multiple machine learning models, including:
  - Decision Tree Classifier
  - XGBoost Classifier
- Performed hyperparameter tuning using RandomizedSearchCV with stratified cross-validation.

### Customer Segmentation
- Applied K-Means clustering to segment customers based on usage and billing behavior.
- Analyzed churn characteristics across different customer segments.

## Model Evaluation
- Prioritized recall as the primary evaluation metric to minimize false negatives.
- Assessed model performance using recall, precision, and overall classification results.

## Key Results
- Customers with month-to-month contracts and higher monthly charges exhibit the highest churn risk.
- The optimized XGBoost model achieved strong recall performance, enabling the identification of most potential churners.
- The model provides actionable insights to support targeted retention campaigns.

## Tools & Technologies
Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, XGBoost
