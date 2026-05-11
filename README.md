# Telecom-Churn-Analysis: Predict behavior to retain customers

## Project Overview
This repository contains the Initial Report, Exploratory Data Analysis (EDA), and Baseline Modeling for the Telecom Churn Prediction project. The primary goal is to identify behavioral "red flags" that indicate a high probability of customer attrition and establish a predictive baseline.

## Project Deliverables
* **Main Jupyter Notebook:** [Telecom_Churn_EDA_Baseline.ipynb](https://github.com/raghu031982/Telecom-Churn-Analysis/blob/main/Telecom_Churn_EDA_Baseline.ipynb)
* **Raw Dataset:** [churn-bigml-20.csv](https://github.com/raghu031982/Telecom-Churn-Analysis/blob/main/churn-bigml-20.csv)

## Summary of Findings
1. **Data Integrity:** The dataset was verified to be exceptionally clean, requiring zero imputation for missing values or duplicate removal.
2. **Behavioral Anomalies:** Utilizing mathematical Interquartile Range (IQR) analysis, the project successfully isolated 57 customers making excessive service calls (>3.5), establishing a primary behavioral indicator of churn risk.
3. **Categorical Risk:** Visual exploratory analysis proves that customers enrolled in an 'International Plan' represent a high-risk cohort with disproportionate churn rates.
4. **Baseline Modeling:** A baseline Decision Tree model was implemented and evaluated via a visual Confusion Matrix and Heatmap to account for heavy class imbalance. It currently achieves a **Recall score of 82.14%**, allowing the business to successfully identify over 8 out of 10 at-risk customers. Moving forward to Module 24, I will implement ensemble techniques to improve this identification rate.
