# Loan Prediction Project

## Overview
This project builds a machine learning model to predict loan approval status based on applicant data. It includes data preprocessing, feature engineering, model training, and evaluation.

## Dataset

<a href='https://www.kaggle.com/datasets/yash9439/loan-prediction/data'>Kaggle Dataset Here</a>

The dataset is loaded from a compressed archive and processed using pandas. Missing values are removed, and categorical variables are encoded for model compatibility.

## Features
Additional features are engineered to improve model performance, including:
- TotalIncome
- Monthly_Payments
- Debt_to_Income
- LoanAmount_to_Income

## Models Used
Several models are evaluated using GridSearchCV:
- Logistic Regression
- Support Vector Machine (SVM)
- Random Forest
- XGBoost

## Training Process
- Data is split into training and test sets
- SMOTE is applied to handle class imbalance
- A pipeline is used for scaling and classification
- Hyperparameters are tuned using cross-validation

## Best Model
The best performing model is a Random Forest classifier with tuned hyperparameters.

## Evaluation
Model performance is evaluated using:
- F1 Score (macro)
- Confusion Matrix
- Classification Report

A probability threshold is also optimized to improve prediction performance.

## Feature Importance
Key features influencing predictions include:
- Credit_History
- TotalIncome
- Debt_to_Income
- LoanAmount

## Requirements
- requirements.txt provided

`%pip install requirements.txt`

## Usage
1. Extract the dataset from the archive
2. Run the preprocessing and training script
3. Evaluate the model using the test set
4. Review performance metrics and feature importance
5. Adjust model accordingly

## Notes
- Ensure the dataset path is correctly set
- Hyperparameter tuning may take time depending on system performance

## License
- MIT License