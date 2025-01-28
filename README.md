# Telecom-churn-prediction
**Overview**

The telecommunication industry is highly competitive, making customer retention a crucial aspect of business growth. This project aims to predict customer churn using machine learning models, enabling telecom operators to identify at-risk customers and take proactive measures to retain them.
The project focuses on building and evaluating classification models like Decision Trees, Random Forests, and Logistic Regression. It also involves data preparation, feature engineering, and model performance comparison to derive actionable insights.

**Dataset Description**
The dataset used in this project contains information about telecom customers, their subscription details, and whether they churned (i.e., discontinued service). It includes 7,043 rows and 21 columns with features like:
**Customer Demographics:** Gender, Senior Citizen status, Partner, Dependents.
**Service Details**: Phone service, Internet service, Streaming services (TV, Movies), etc.
**Contract Information:** Contract type (Month-to-Month, One year, Two year), Payment method, Paperless billing.
**Billing Information:** Monthly charges, Total charges.
**Target Variable:** Churn (Yes/No).

**Key Features and Insights**

**Data Exploration:**

High churn is observed among customers with month-to-month contracts, no online security, and those in the first year of subscription.

Low churn is associated with long-term contracts and customers engaged for more than five years.

Gender, phone service, and multiple lines have minimal impact on churn.

**Data Preprocessing:**

Converted Total Charges to numeric format and handled missing values.

**Machine Learning Models**

Three machine learning models were implemented and evaluated:

**1. Decision Tree**

Accuracy: 94%

Precision and Recall:

Class 0: Precision 0.95, Recall 0.92

Class 1: Precision 0.93, Recall 0.96

**2. Random Forest**

Accuracy: 95%

Precision and Recall:

Class 0: Precision 0.97, Recall 0.91

Class 1: Precision 0.93, Recall 0.98

**3. Logistic Regression**

Accuracy: 95%

Precision and Recall:

Class 0: Precision 0.94, Recall 0.94

Class 1: Precision 0.95, Recall 0.95
Created tenure groups to categorize customers based on their subscription length.

**Feature Engineering:**

Removed redundant columns like Customer ID.

Used SMOTEENN (Synthetic Minority Oversampling + Edited Nearest Neighbors) for handling class imbalance.

**Results and Recommendations**

Best Model: Both Random Forest and Logistic Regression achieved 95% accuracy. Random Forest slightly outperformed in terms of recall for churned customers.

Business Insight: Telecom operators should focus on:

Encouraging long-term contracts.

Providing online security and tech support services.

Engaging new customers effectively during their first year.
