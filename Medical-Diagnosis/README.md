# Medical Diagnosis Prediction

## Project Overview

This project focuses on predicting the likelihood of a medical diagnosis using patient demographic information, health characteristics, and biomarker measurements. By applying machine learning classification techniques, the project aims to identify patterns associated with disease presence and evaluate the effectiveness of different predictive models in a healthcare setting.

## Dataset Information

The dataset contains patient demographic characteristics, lifestyle information, family medical history, and ten biomarker measurements. The target variable indicates whether a patient is healthy or has a diagnosed medical condition.

Key features include:

* Age
* Gender
* Family History
* Lifestyle Score
* Biomarker 1–10
* Diagnosis (Healthy vs Disease)

## Objective

The primary objective of this project is to develop machine learning models capable of predicting medical diagnoses based on patient characteristics and biomarker data. In healthcare applications, accurately identifying patients with disease is critical, making sensitivity (recall) an important evaluation metric.

## Approach

The project followed a structured machine learning workflow:

### Data Exploration

* Performed exploratory data analysis to understand dataset structure and class distribution.
* Examined correlations between biomarkers and disease diagnosis.
* Created visualizations to identify patterns and relationships within the data.

### Data Preparation

* Selected relevant demographic, lifestyle, and biomarker features.
* Encoded categorical variables into numerical values.
* Standardized features using StandardScaler to improve model performance.
* Split the dataset into training and testing sets.

### Model Development

Several classification algorithms were developed and evaluated:

* Logistic Regression
* K-Nearest Neighbors (KNN)
* Support Vector Machine (SVM)
* Decision Tree Classification

Cross-validation techniques were used to evaluate model performance and reduce the risk of overfitting.

### Model Evaluation

Models were assessed using:

* Accuracy
* Precision
* Recall (Sensitivity)
* F1-Score
* 5-Fold Cross-Validation

Because medical diagnosis prioritizes identifying patients with disease, recall was emphasized as a key performance metric.

## Results

The Decision Tree model achieved the strongest performance, producing a recall score of approximately 54.3% under 5-fold cross-validation.

Model comparison demonstrated that the Decision Tree was the most effective at identifying positive diagnoses while maintaining a reasonable balance between precision and recall. Logistic Regression and KNN achieved moderate performance, while SVM showed the lowest recall among the evaluated models.

## Medical Insights

The analysis revealed that Biomarker 1, Biomarker 2, and Biomarker 3 were the strongest predictors of disease diagnosis.

From a healthcare perspective, minimizing false negatives is critical because missed diagnoses can delay treatment and negatively impact patient outcomes. While the Decision Tree achieved the highest sensitivity, the results also highlight the challenges of medical prediction and the importance of continuing to improve diagnostic accuracy.

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

