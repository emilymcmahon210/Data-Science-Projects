# Customer Churn Prediction

## Project Overview

Customer retention is a critical challenge for subscription-based businesses, as acquiring new customers is often more expensive than retaining existing ones. This project focuses on predicting customer churn and identifying the customer characteristics most strongly associated with attrition. By understanding which customers are most likely to leave, organizations can implement targeted retention strategies and reduce revenue loss.

## Key Results

- Decision Tree achieved the highest performance with 73.5% accuracy and an AUC-ROC score of 0.782.
- Contract type, monthly charges, and tenure were the strongest predictors of customer churn.
- Customers with Contract Type 0 exhibited nearly three times the churn rate of customers with longer-term contracts.

## Dataset Information

The dataset contains customer demographic information, account details, service subscriptions, and contract information. Features include customer tenure, age, contract type, internet service, monthly charges, payment methods, and additional service options.

The target variable indicates whether a customer churned (canceled service) or remained with the company.

## Objective

The primary objective of this project is to develop machine learning models capable of predicting customer churn while identifying the factors that contribute most significantly to customer attrition. The results can help businesses proactively target at-risk customers and improve retention efforts.

## Approach

The project followed a structured machine learning workflow:

### Data Exploration

To better understand customer behavior, churn rates were analyzed across key service categories.

#### Churn Rate by Contract Type

<img width="619" height="383" alt="image" src="https://github.com/user-attachments/assets/4a688fe2-2f28-408e-931c-727754477517" />


Customers with Contract Type 0 exhibited the highest churn rate at approximately 45%, while customers with Contract Types 1 and 2 experienced substantially lower churn rates of approximately 16%. This suggests that contract structure is strongly associated with customer retention and may be an important predictor of churn.

#### Churn by Internet Service

<img width="566" height="386" alt="image" src="https://github.com/user-attachments/assets/e26ff1f8-477b-471a-8464-250a9d25fdee" />

Customers in Internet Service Category 2 exhibited substantially higher churn rates than customers in Categories 0 and 1, suggesting that service type may be an important predictor of customer attrition.


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

### Model Evaluation

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* AUC-ROC

Performance metrics were compared to determine the most effective model for churn prediction.

## Results

### Model Performance Comparison

<img width="1260" height="445" alt="image" src="https://github.com/user-attachments/assets/c7eee56e-9e42-4abb-978e-51964d5a36d4" />

The ROC and Precision-Recall curves demonstrate the performance of each classification model across multiple decision thresholds. The Decision Tree achieved the highest overall discrimination ability with an AUC-ROC score of 0.782, followed closely by Logistic Regression (0.771). KNN produced the weakest performance across both evaluation curves.

### Model Comparison Metrics

<img width="523" height="93" alt="image" src="https://github.com/user-attachments/assets/e1cf895c-36a1-4351-8975-ca3eb1feac5b" />

The Decision Tree model achieved the strongest overall performance, with the highest accuracy (73.5%), recall (48.9%), F1-score (0.543), and AUC-ROC score (0.782). While Logistic Regression performed similarly, the Decision Tree provided the best balance between identifying churned customers and minimizing classification errors.


### Feature Importance

<img width="869" height="473" alt="image" src="https://github.com/user-attachments/assets/71b31faa-024f-4878-839d-d9b67be2c9b0" />

Contract type, monthly charges, tenure, and total charges were identified as the most influential predictors of customer churn. These findings suggest that customer commitment level and service costs play a major role in retention outcomes.

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
