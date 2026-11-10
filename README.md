# AI-Powered Customer Churn Prediction & Retention Intelligence

## Project Overview

This project develops a machine learning-based customer churn prediction system using the IBM Telco Customer Churn dataset.

It analyses customer behaviour, identifies factors associated with customer attrition, predicts churn probability and translates model predictions into actionable customer retention insights.

The project combines exploratory data analysis, feature engineering, classification algorithms, hyperparameter tuning and explainable AI.

## Objectives

- Identify customers who are likely to discontinue a service.
- Explore behavioural and financial factors associated with churn.
- Train and compare multiple machine learning models.
- Improve prediction performance through threshold optimisation.
- Interpret model predictions using SHAP explainability.
- Segment customers into different churn-risk categories.
- Develop data-driven customer retention recommendations.

## Dataset

**Source:** IBM Telco Customer Churn public sample dataset.

- 7,043 customer records
- 21 original features
- Customer demographics, services, contracts, payment methods and billing information
- Binary target variable: Churn

## Technologies Used

- Python
- Jupyter Notebook
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- SHAP (Explainable AI)

## Project Workflow

### 1. Data Collection
Load the publicly available IBM Telco Customer Churn dataset.

### 2. Exploratory Data Analysis
Examine customer demographics, service subscriptions, contract types, billing patterns and churn distribution.

### 3. Data Preprocessing
Clean the dataset, handle missing or inconsistent values and prepare categorical and numerical features.

### 4. Feature Engineering
Transform relevant customer attributes into machine learning features.

### 5. Model Development
Train and compare:
- Logistic Regression
- Random Forest
- Gradient Boosting

### 6. Model Evaluation
Evaluate models using:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

### 7. Threshold Optimisation
Compare prediction thresholds to balance churn detection and false positives.

### 8. Explainable AI
Use SHAP to identify important features influencing churn predictions and improve model interpretability.

### 9. Customer Retention Intelligence
Classify customers into low-, medium- and high-risk categories and generate retention-oriented insights.

## Model Results

The tuned Logistic Regression model at a classification threshold of 0.35 achieved:

| Evaluation Metric | Result |
|---|---:|
| Accuracy | 78.28% |
| Precision | 57.14% |
| Recall | 72.73% |
| F1-score | 64.00% |
| ROC-AUC | 84.66% |
| Balanced Accuracy | 76.51% |

Threshold selection prioritises churn detection by improving recall, while accepting a trade-off in precision and accuracy.

These are experimental development results, not independently validated final performance.

## Explainability Insights

SHAP analysis was used to investigate the contribution of customer features to churn predictions.

Important factors included:
- Contract type
- Customer tenure
- Internet service type
- Payment method
- Monthly charges
- Online security subscription

## Customer Risk Segmentation

The model's predictions were used to categorise customers into three risk groups:

- Low Risk
- Medium Risk
- High Risk

This provides a foundation for prioritising customer retention efforts.

## Limitations and Future Scope

- The model uses a publicly available telecommunications dataset.
- Test-set results were inspected during iterative development; an untouched holdout set or nested cross-validation would be required for independent validation.
- Predictions reflect patterns in historical data and do not establish causation.
- Future improvements could include deployment through Streamlit, real-time churn monitoring and cost-sensitive retention strategies.

## Disclaimer

This is an independent educational machine learning project using publicly available data. It is not affiliated with or endorsed by IBM, Morgan Stanley or any other financial institution.

## Author

**Ananya Jhaveri**

B.Tech – Artificial Intelligence and Data Science
