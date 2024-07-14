# Credit-Scoring-Classification

## Overview
This project aims to develop a credit scoring model using historical banking data. The goal is to predict the credit score of customers based on various features. The project involves several steps, including data exploration, data preprocessing, feature engineering, feature selection, model building, evaluation, and application on new data.

## Table of Contents
- Introduction
- Data Exploration
- Data Preprocessing
- Feature Engineering
- Model Building
- Model Evaluation
- Applying Model on New Data
- Conclusion


## Introduction
Credit scoring is a crucial task in the banking and financial sectors, enabling institutions to evaluate the creditworthiness of potential borrowers. This project uses a dataset containing various features related to customer information and loan details to build a predictive model.

## Data Exploration
The dataset comprises multiple features, including numerical and categorical data. Initial exploration revealed insights into the structure and summary statistics of the data.

- Rows and Columns: 100,000 rows and 28 columns
- Data Types: Mixed data types, including integers, floats, and objects
- Missing Values: Various columns with missing values were identified and addressed

## Data Preprocessing
To ensure the data was clean and suitable for modeling, several preprocessing steps were undertaken:

- Unwanted Characters Removal: Stripped and replaced unwanted characters
- Missing Value Imputation: Filled missing values using group modes and custom values
- Data Type Conversion: Converted columns to appropriate data types

## Feature Engineering
Feature engineering involved transforming existing features and creating new ones to improve the model's predictive power:
- Credit History Age: Converted from years and months to total months
- Outlier Capping: Applied the IQR method to cap outliers

## Model Building
The model used for this project was Random Forest Classifier. It was the best performing model after testing various machine learning models
The model was trained and evaluated using an 70-30 train-test split.

## Model Evaluation
The performance of the models was evaluated using various metrics:
RandomForest Classifier:
Accuracy: 0.86

Classification Report
              precision    recall  f1-score   support

           1       0.86      0.88      0.87     16014
           2       0.84      0.76      0.80     15952
           3       0.87      0.93      0.90     15891

    accuracy                           0.86     47857
   macro avg       0.86      0.86      0.86     47857
weighted avg       0.86      0.86      0.86     47857

## Applying Model on New Data
The trained model was applied to a new dataset to predict credit scores. The new data underwent the same preprocessing and feature engineering steps as the training data.

## Conclusion
This project successfully developed and evaluated credit scoring models using RandomForest. The models demonstrated good accuracy and robustness. Future improvements could include exploring additional feature engineering techniques, hyperparameter tuning, and incorporating domain-specific knowledge to enhance model performance.
