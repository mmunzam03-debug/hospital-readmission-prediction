# hospital-readmission-prediction
Overview

This project builds machine learning models to predict whether a patient will be readmitted to a hospital within 30 days. The goal is to identify high-risk patients who may benefit from additional monitoring or intervention.

Problem

Hospital readmissions are costly and often preventable. The dataset is highly imbalanced, with most patients not being readmitted, making it challenging to correctly identify high-risk cases.

Approach

1. Cleaned and preprocessed healthcare dataset

2. Handled missing values and removed data leakage

3. Performed feature engineering (e.g., grouping diagnosis codes into medical categories)

4. Converted categorical variables using one-hot encoding

5. Addressed class imbalance using class weights and scaling

Models Used

1. Logistic Regression

2. Random Forest

3. XGBoost

Key Results

1. Random Forest achieved high accuracy but failed to detect readmissions due to class imbalance

2. XGBoost significantly improved recall (54%), making it more effective for identifying high-risk patients

3. Explored precision-recall tradeoff to adjust model threshold based on real-world priorities

Key Insights

1. Features such as number of inpatient visits, medications, and lab procedures strongly influenced readmission risk

2. There is a tradeoff between precision and recall — improving detection of high-risk patients increases false positives

3. Model can be used as a screening tool rather than a final decision system

Tools & Technologies

Python, Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn, SHAP

Future Improvements

1. Improve feature selection and domain specific variables

2. Experiment with additional models and ensemble methods

2. Integrate into a real-time clinical decision support system
