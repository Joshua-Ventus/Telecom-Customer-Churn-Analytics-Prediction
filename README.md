# Telecom Customer Churn Analytics & Prediction

## Overview

Customer churn is one of the most significant challenges faced by telecommunications companies. Acquiring a new customer is often more expensive than retaining an existing one, making customer retention a critical business objective.

This project develops a machine learning-based churn prediction system that identifies customers who are likely to discontinue their services. By leveraging customer demographics, usage behavior, revenue patterns, and service-related information, the solution provides actionable insights that enable proactive customer retention strategies.

---

## Business Problem

Telecommunication companies experience revenue losses when customers switch to competitors or terminate their subscriptions. The ability to identify high-risk customers before they churn can help organizations:

* Reduce customer attrition.
* Improve customer satisfaction.
* Increase customer lifetime value.
* Optimize retention campaign investments.
* Protect recurring revenue streams.

The goal of this project is to build a predictive model capable of accurately identifying customers at risk of churn and generating business recommendations based on the findings.

---

## Dataset Description

The dataset consists of customer demographic information, service usage records, billing data, and network-related metrics.

### Data Sources

The project combines:

* Customer profile data
* Service usage data
* Revenue and billing information
* Customer account information

### Example Features

| Feature       | Description                |
| ------------- | -------------------------- |
| months        | Customer tenure            |
| mou_Mean      | Average minutes of usage   |
| rev_Mean      | Average customer revenue   |
| totmrc_Mean   | Monthly recurring charge   |
| change_mou    | Change in usage behavior   |
| change_rev    | Change in customer revenue |
| ovrrev_Mean   | Average overage revenue    |
| drop_blk_Mean | Dropped and blocked calls  |
| hnd_webcap    | Handset web capability     |
| marital       | Marital status             |
| churn         | Target variable            |

---

## Project Workflow

### 1. Data Integration

* Merged customer and usage datasets using Customer_ID.
* Validated data consistency and completeness.

### 2. Data Cleaning

* Handled missing values.
* Treated inconsistent categorical values.
* Removed duplicate records.
* Performed data quality checks.

### 3. Exploratory Data Analysis (EDA)

Conducted analysis to understand:

* Churn distribution
* Customer demographics
* Revenue patterns
* Usage trends
* Service quality indicators
* Customer tenure characteristics

### 4. Feature Engineering

Created and transformed features related to:

* Customer engagement
* Revenue behavior
* Service utilization
* Usage changes
* Network quality metrics

Applied:

* Frequency Encoding
* One-Hot Encoding
* Label Encoding (where appropriate)

### 5. Model Development

Built and evaluated multiple machine learning models including:

* Logistic Regression
* Random Forest
* XGBoost
* LightGBM
* Gradient Boosting

Hyperparameter tuning and cross-validation were used to improve model performance.

---

## Model Evaluation

The models were assessed using:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC

These metrics were used to evaluate the model's ability to identify churners while minimizing false predictions.

---

## Key Findings

Feature importance analysis identified several strong churn indicators:

* Customer tenure (`months`)
* Monthly recurring charges (`totmrc_Mean`)
* Changes in customer usage (`change_mou`)
* Revenue trends (`change_rev`)
* Service quality metrics
* Network experience indicators

Customers with declining engagement, decreasing revenue, and shorter tenure were found to be at a higher risk of churn.

---

## Business Recommendations

Based on the analytical findings, a business proposal was developed to support customer retention initiatives.

patterns as leading churn indicators.

### Expected Benefits

* Reduced customer churn.
* Increased customer retention.
* Improved customer lifetime value.
* Enhanced revenue stability.
* More efficient allocation of retention resources.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* XGBoost
* LightGBM
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Repository Structure

```text
Telecom-Churn-Prediction/
│
├── data/
│   ├── customer_data.csv
│   └── usage_data.csv
│
├── notebooks/
│   └── Telecom_Churn_Analysis.ipynb
│
├── models/
│
├── images/
│
├── README.md
│
└── requirements.txt
```

---

## Future Improvements

* Deploy the model as a web application.
* Implement automated model retraining pipelines.
* Incorporate customer interaction and support data.
* Develop real-time churn prediction capabilities.
* Integrate explainable AI techniques for model interpretability.

---

## Author

**Joshua Aniehe**

Data Analytics | Machine Learning | Predictive Modeling | Business Intelligence

Focused on building data-driven solutions that transform business challenges into actionable insights and measurable outcomes.
# Telecom-Customer-Churn-Analytics-Prediction
Built an end-to-end machine learning solution to predict customer churn using demographic, revenue, usage, and service-quality data. Performed feature engineering, model optimization, and feature importance analysis to identify key churn drivers
