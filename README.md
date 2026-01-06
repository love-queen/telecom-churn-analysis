# Telco Customer Churn – ML Case Study

This repository contains an end‑to‑end machine learning project that predicts customer churn for a telecom company.

## Project overview

The goal is to identify customers who are likely to churn so that the business can proactively retain them with targeted offers and interventions. The notebook walks through problem framing, exploratory data analysis, feature engineering, model training, and business insights.

## Dataset

The project uses the `WA_Fn-UseC_-Telco-Customer-Churn-2.csv` dataset, which includes: 

- Customer demographics (gender, senior citizen, dependents, etc.).
- Service information (phone, internet, contract type, payment method, additional services).
- Billing details (monthly charges, total charges). 
- Target variable: `Churn` indicating whether the customer left (Yes/No).

## Methods

Main steps implemented in the notebook:

- Data cleaning and type fixing (e.g., converting `TotalCharges` to numeric and handling missing values).
- Exploratory data analysis:
  - Overall churn rate.
  - Churn by contract type, internet service, tenure, and charges.
- Feature engineering:
  - Tenure groups.
  - Engagement features such as number of add‑on services.
  - Flags for new customers and high monthly charges.
- Modeling:
  - Train/test split with stratification.
  - Preprocessing pipeline with One‑Hot Encoding for categorical features.
  - Logistic Regression and Random Forest classifiers.
- Evaluation:
  - Confusion matrix and classification report.
  - ROC curves and ROC‑AUC for both models.
  - Focus on recall/precision for churners (positive class).
- Post‑model analysis:
  - Inspection of false positives and false negatives.
  - Segment analysis by contract, internet service, tenure group, and payment method.
