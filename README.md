# Predicting Customer Churn in Telecom Services

## Project Overview
This project aimed to predict the likelihood of customer attrition (churn) using advanced machine learning models. By analyzing service usage, plan subscriptions, and support interactions, I identified the key behavioral "red flags" that indicate a high probability of a customer leaving. The goal of this analysis is to provide actionable intelligence that allows retention teams to transition from reactive support to proactive customer success, ultimately maximizing Customer Lifetime Value (CLV).

The dataset, sourced from BigML and available via [Kaggle](https://www.kaggle.com/datasets/mnassrib/telecom-churn-datasets), contains anonymized account details, behavioral metrics, and support history.

## Notebooks
-[Telecom_Churn_Final_Capstone.ipynb](https://colab.research.google.com/drive/1X9jCLViblv0gQReZSSEFZZi7Sdg88Ua9?usp=sharing) – The comprehensive pipeline covering the full analysis, from data acquisition to model export.

## Key Features Considered
- Account & Plan details (e.g., International plan enrollment, account length)
- Behavioral Usage metrics (e.g., Total minutes, calls, and charges segmented by time of day)
- Customer Support interactions (e.g., Frequency of customer service calls)

## Project Workflow
The project followed a structured ML pipeline, which included:
1. Problem Statement & Business Objective
2. Data Acquisition & Setup
3. Data Preprocessing & Targeted EDA
4. Phase I Modeling: The "Wide Net" Algorithmic Funnel
5. Phase II Modeling: Complex Hyperparameter Tuning & Pipelines
6. Model Evaluation: The Precision-Recall Trade-Off
7. Model Interpretation (SHAP) & Live Case Study
8. Conclusion, Business Recommendations & Model Export

## Key Findings
- Customer Service Calls are the #1 predictor – A high volume of support interactions is the most significant behavioral indicator of immediate churn risk.
- International Plan correlation – Customers enrolled in the International Plan show disproportionately higher churn rates.
- Model Performance – The tuned XGBoost model achieves a robust Recall score of 0.7241, ensuring that the majority of at-risk customers are identified.
- Predictive Transparency – SHAP interpretation confirms that churn is driven by identifiable patterns—specifically high usage intensity and support interaction frequency rather than random noise.

## Business & Strategic Recommendations
To improve customer retention, I recommend the following:
- Implement Proactive Outreach – Trigger loyalty intervention immediately after a customer exceeds 3 service interactions.
- Review International Plan Strategy – Evaluate whether current International Plan pricing or coverage is meeting customer expectations, given the higher churn in this segment.
- Automate Risk Scoring – Integrate the exported model into the CRM to score customers monthly and prioritize "High-Risk" individuals for proactive loyalty rewards.
- Leverage Predictive Insights – Transition from reactive support to proactive retention using model-driven behavioral alerts.

## Tech Stack
- Python: pandas, NumPy, scikit-learn, XGBoost, SHAP
- Data Visualization: Matplotlib, Seaborn
- Machine Learning Techniques: Pipeline, GridSearchCV, Stratified K-Fold
- Model Deployment: joblib

## Project Contributors
- Raghubendra Dagur, Managing Director at SciBiz Consulting, LLC
- This project was completed as part of the final capstone for the Professional Certificate in Machine Learning and Artificial Intelligence, UC Berkeley, under the supervision of Instructor Ahmet F. Cakmak, PhD.
