# Customer Churn Prediction

## Project Overview

Customer retention is a critical challenge for subscription-based businesses, as acquiring new customers is often more expensive than retaining existing ones. This project focuses on predicting customer churn and identifying the customer characteristics most strongly associated with attrition. By understanding which customers are most likely to leave, organizations can implement targeted retention strategies and reduce revenue loss.

## Dataset Information

The dataset contains customer demographic information, account details, service subscriptions, and contract information. Features include customer tenure, age, contract type, internet service, monthly charges, payment methods, and additional service options.

The target variable indicates whether a customer churned (canceled service) or remained with the company.

## Objective

The primary objective of this project is to develop machine learning models capable of predicting customer churn while identifying the factors that contribute most significantly to customer attrition. The results can help businesses proactively target at-risk customers and improve retention efforts.

## Approach

The project followed a structured machine learning workflow:

### Data Exploration

* Performed exploratory data analysis to understand customer demographics and service usage patterns.
* Calculated churn rates by contract type and internet service type.
* Created visualizations to identify customer segments with higher churn risk.

### Data Preparation

* Selected relevant demographic, account, and service-related features.
* Encoded categorical variables into numerical values.
* Standardized features using StandardScaler where appropriate.
* Split the data into training and testing datasets.

### Model Development

Several machine learning classification models were developed and compared:

* Logistic Regression
* K-Nearest Neighbors (KNN)
* Support Vector Machine (SVM)
* Decision Tree Classification

### Feature Importance Analysis

Feature importance was evaluated using Logistic Regression coefficients and Decision Tree importance scores to identify the strongest predictors of churn.

### Model Evaluation

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* AUC-ROC

Performance metrics were compared to determine the most effective model for churn prediction.

## Results

The Decision Tree model achieved the strongest overall performance with:

* Accuracy: 73.5%
* AUC-ROC: 0.78

Model comparison demonstrated that Decision Trees provided the best balance between predictive performance and interpretability.

Feature importance analysis identified several key drivers of churn, including:

* Customer tenure
* Contract type
* Internet service
* Online security services

These findings suggest that contract structure and service utilization play a significant role in customer retention.

## Business Impact

Customer churn prediction allows organizations to identify high-risk customers before cancellation occurs. The insights generated from this analysis can support:

* Customer retention campaigns
* Personalized service offerings
* Contract optimization strategies
* Revenue protection initiatives

By proactively addressing churn risk, businesses can improve customer satisfaction and reduce the costs associated with customer acquisition.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Logistic Regression
* K-Nearest Neighbors (KNN)
* Support Vector Machine (SVM)
* Decision Tree Classification
* Cross Validation
