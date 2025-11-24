# Credit Risk Prediction

## Project Overview:
A machine learning project to predict credit card default risk using customer demographics, bill amounts, and past payment behavior.
The goal is to help financial institutions identify high-risk clients before issuing or extending credit.


## Dataset:

- **Source:** UCI Machine Learning Repository
- **Samples:** 30,000 customers
- **Features:** 24 (payment history, bill amounts, credit limit, demographics)
- **Target:** default_next_month (1 = default, 0 = no default)


## Models & Results
| Model                   | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|-------------------------|----------|-----------|--------|----------|---------|
| XGBoost                 | 0.8177   | 0.6589    | 0.3640 | 0.4689   | 0.7734  |
| Support Vector Machine  | 0.8170   | 0.6880    | 0.3158 | 0.4329   | 0.7250  |
| Random Forest           | 0.7957   | 0.5375    | 0.5448 | 0.5412   | 0.7720  |
| Logistic Regression     | 0.7732   | 0.4887    | 0.5554 | 0.5199   | 0.7590  |


## Key Findings:

- **Best Model:** XGBoost (highest accuracy and ROC-AUC)
- **Most Important Features:** payment delays, bill amount history, credit utilization
- **Business Value:** can identify 43% of potential defaulters with 77% precision

## Project Structure:
- credit_risk_model/
- ├── data/            # Raw and processed datasets
- ├── models/          # Trained model files (.pkl)
- ├── notebooks/       # Cleaning, EDA, preprocessing, modeling
- ├── requirements.txt
- └── README.md
