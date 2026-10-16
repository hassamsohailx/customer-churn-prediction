# Customer Churn Prediction Using Machine Learning

A Bachelor’s thesis project exploring how machine learning can identify customers at risk of churn in subscription-based businesses. The project combines exploratory data analysis, data preprocessing, predictive modelling, and model performance evaluation using the IBM Telco Customer Churn dataset.

## Project Overview

Customer churn is a major challenge for subscription-based businesses. This project investigates how machine learning models can identify customer characteristics associated with churn and support data-driven customer retention strategies.

The research compares four supervised classification algorithms and evaluates their predictive performance using multiple classification metrics.

## Research Objectives

- Explore customer demographics, subscription behaviour, services, and financial characteristics.
- Clean and preprocess the dataset for machine learning.
- Investigate patterns and factors associated with customer churn.
- Train and compare four classification models.
- Evaluate model performance using accuracy, precision, recall, F1-score, and ROC-AUC.
- Interpret important churn predictors and discuss their business implications.

## Dataset

**Source:** IBM Telco Customer Churn dataset, obtained through Kaggle.

- **Customer records:** 7,043
- **Variables:** 21
- **Target variable:** `Churn`
- **Problem type:** Binary classification

The dataset includes customer demographics, contract types, subscription tenure, service usage, payment methods, and billing information.

## Tools & Technologies

- **Python** — data analysis and model development
- **Pandas** — data manipulation and preprocessing
- **NumPy** — numerical operations
- **Matplotlib** — data visualization
- **Scikit-learn** — classification models and evaluation
- **XGBoost** — gradient-boosting classification
- **SMOTE** — handling class imbalance in the training data

## Methodology

1. **Exploratory Data Analysis (EDA):** Examined customer characteristics and patterns associated with churn.
2. **Data Preprocessing:** Addressed missing values, encoded categorical variables, and standardized numerical features.
3. **Class Balancing:** Applied Synthetic Minority Over-sampling Technique (SMOTE) to the training data.
4. **Model Development:** Trained and compared Logistic Regression, Decision Tree, Random Forest, and XGBoost.
5. **Model Evaluation:** Compared accuracy, precision, recall, F1-score, confusion matrices, and ROC-AUC.
6. **Feature Importance:** Investigated customer characteristics associated with churn risk.

## Model Performance

The following results are reported in the bachelor thesis.

| Model | Accuracy | Precision | Recall | F1-score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 74.24% | 50.95% | 78.88% | 61.91% | 83.90% |
| Decision Tree | 71.89% | 47.49% | 55.61% | 51.23% | 66.71% |
| Random Forest | 76.93% | 56.22% | 58.02% | 57.11% | 82.22% |
| XGBoost | 77.50% | 57.25% | 60.16% | 58.67% | 81.44% |

### Key Findings

- **XGBoost** achieved the highest accuracy at 77.50%, with the highest precision among the four models.
- **Logistic Regression** achieved the highest recall (78.88%), F1-score (61.91%), and ROC-AUC (83.90%).
- **Random Forest** delivered the second-highest accuracy at 76.93%.
- **Decision Tree** recorded the lowest accuracy and ROC-AUC among the evaluated models.
- Contract type, tenure, monthly charges, total charges, online security, and technical support were identified as important churn-related factors.

These results illustrate why model selection should depend on the business objective: overall classification accuracy and identifying as many at-risk customers as possible are not the same goal.

## Business Implications

The findings suggest that subscription-based businesses could use churn prediction to:

- Identify customers who may be at risk of leaving.
- Investigate retention strategies for customers on month-to-month contracts.
- Evaluate the role of pricing, service quality, online security, and technical support.
- Support customer segmentation and evidence-based retention decisions.

Predictive models should support, rather than replace, business judgment and responsible customer management.

## Project Files

- **Jupyter Notebook (`.ipynb`):** Python code and analysis.
- **Thesis (`.pdf`):** Full academic research, methodology, results, and discussion.
- **Dataset (`.csv`):** Customer data used for the analysis.

## Limitations

The findings are based on a single telecom customer dataset and four supervised classification algorithms. Results may differ across businesses, datasets, and customer populations. Model performance also depends on preprocessing choices and the evaluation setup.

## Author

**Hassam Sohail**  
Bachelor's in Digital Business and Data Science

This project was completed as part of my bachelor's thesis.
