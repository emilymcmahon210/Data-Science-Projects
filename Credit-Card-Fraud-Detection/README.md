# Credit Card Fraud Detection

## Project Overview

Credit card fraud poses a significant challenge for financial institutions due to the volume of transactions processed daily and the relatively small number of fraudulent events. This project focuses on identifying potentially fraudulent credit card transactions using machine learning classification techniques and evaluating model performance in a highly imbalanced dataset.

## Dataset Information

The dataset contains historical credit card transaction data labeled as either legitimate or fraudulent. Because fraudulent transactions represent only a small fraction of all transactions, the dataset presents a class imbalance problem commonly encountered in real-world fraud detection systems.

The available features describe transaction characteristics that may help distinguish fraudulent behavior from legitimate customer activity.

## Objective

The primary objective of this project is to develop machine learning models capable of detecting fraudulent transactions while minimizing missed fraud cases. Since fraudulent transactions are rare, traditional accuracy metrics can be misleading, making recall and AUC-ROC important measures of model effectiveness.

## Approach

The project followed a structured machine learning workflow:

### Data Exploration

* Examined the distribution of fraudulent and legitimate transactions.
* Analyzed class imbalance and its potential impact on model performance.
* Explored transaction patterns associated with fraudulent activity.

### Data Preparation

* Cleaned and prepared the dataset for machine learning analysis.
* Selected relevant features for model training.
* Split the dataset into training and testing datasets.

### Model Development

Two classification models were developed and compared:

* Logistic Regression
* Support Vector Machine (SVM)

### Model Evaluation

Models were evaluated using:

* Precision
* Recall
* F1-Score
* AUC-ROC

Particular emphasis was placed on recall, as missed fraudulent transactions (false negatives) can result in significant financial losses.

## Results

The Logistic Regression model achieved the strongest overall performance:

* Recall: 33.3%
* AUC-ROC: 0.47

Compared to SVM, Logistic Regression identified a larger proportion of fraudulent transactions and demonstrated superior fraud detection capability within the dataset. The results also highlighted the challenges associated with highly imbalanced datasets, where accurately detecting rare fraud events remains difficult even when using advanced machine learning techniques.

Model Performance Interpretation: The confusion matrices reveal the challenges of detecting fraudulent transactions in a highly imbalanced dataset. While Logistic Regression identified the greatest number of fraudulent transactions (10 true positives), all models struggled to detect the minority class. The Random Forest model failed to identify any fraudulent transactions, while SVM detected only 4 fraud cases. These results demonstrate that high overall accuracy can be misleading in fraud detection problems and highlight the importance of evaluating models using recall and false negative rates.

<img width="1299" height="406" alt="image" src="https://github.com/user-attachments/assets/4f6086b5-e5f3-48b5-8811-07f1d8ea8ad7" />



## Key Findings

* Fraud detection is significantly impacted by class imbalance.
* Recall is a critical metric because missed fraud cases can be costly.
* Logistic Regression outperformed SVM in identifying fraudulent transactions.
* Additional techniques such as resampling, class weighting, or ensemble methods may improve future model performance.

## Business Impact

Fraud detection systems play a critical role in reducing financial losses, protecting customers, and maintaining trust in financial institutions. Although fraud events are rare, accurately identifying suspicious transactions can significantly reduce risk exposure and support more effective fraud prevention strategies.

This project demonstrates the challenges of real-world fraud detection and highlights the importance of selecting evaluation metrics that align with business objectives.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Logistic Regression
* Support Vector Machine (SVM)
* Classification Metrics
* Imbalanced Data Analysis
