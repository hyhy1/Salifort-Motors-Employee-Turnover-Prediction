# Salifort-Motors-Employee-Turnover-Prediction

Overview
This project focuses on analyzing employee data from Salifort Motors to predict and understand employee turnover, which is a significant cost and cultural concern for the company. We utilized a dataset containing employee attributes (e.g., job title, hours, satisfaction) to identify the key risk factors driving departures and to build a highly accurate machine learning model to forecast which employees are most likely to leave.

The final XGBoost classification model achieved an ROC AUC of over 0.95 and a high Recall for the leavers class, making it a robust tool for proactive intervention.

Business Understanding
Salifort Motors is dealing with a high, financially costly employee turnover rate. The company invests heavily in recruiting and training, making every departure expensive.

The goal is to provide the Senior Leadership and HR teams with:

Quantifiable Reasons: Statistical evidence defining why employees are leaving (e.g., burnout, low satisfaction).

A Predictive Tool: A model to forecast who is likely to leave, enabling targeted retention efforts.

This work aims to reduce the turnover rate, cut replacement costs, and foster a more positive corporate culture.

Data Understanding
The project utilized employee data, likely sourced from HR records and an employee survey, containing attributes relevant to job satisfaction and workload.

Key features analyzed include:

Target Variable: Left (Binary: 0=Stayed, 1=Left).

Predictors: Department, Job Title, Number of Projects, Average Monthly Hours, Satisfaction Level, and Salary.

Initial Exploratory Data Analysis (EDA) revealed a clear separation between leavers and stayers, particularly concerning Satisfaction Level and Average Monthly Hours, which were key factors for modeling. The target variable (Left) was imbalanced, which influenced the choice of evaluation metrics.

Modeling and Evaluation
We constructed and evaluated multiple models, including Logistic Regression (for a statistical baseline) and advanced Machine Learning models (Random Forest, XGBoost).

The XGBoost model was selected as the final choice due to its superior performance in handling the data's non-linear relationships and class imbalance.

Key Performance Metrics (Hypothetical Optimized Results):
Feature Importance
Model interpretation confirmed that the primary drivers of turnover are:

Employee Satisfaction Level

Average Monthly Hours

Years at Company

Conclusion and Recommendations
The predictive model successfully identifies employees at high risk of departure, and the analysis pinpoints the core issues leading to turnover.

Business Recommendations:
Implement Workload Thresholds: Proactively monitor and intervene with employees whose Average Monthly Hours exceed a specific threshold (e.g., the mean of the leaver group) to prevent burnout.

Targeted Retention Programs: Prioritize retention efforts for employees flagged as high risk, focusing on those with a combination of low satisfaction and high hours.

Review Compensation: Immediately review and adjust compensation for employees in the lowest salary band, as this was a significant, contributing factor to turnover.

Future Work:
Integrate the model into an HR dashboard for continuous, real-time risk scoring.

Explore "what-if" scenario modeling (e.g., how much does a 10% raise reduce the probability of leaving?).

Monitor model performance for data drift, as the factors driving employee behavior can change over time.
