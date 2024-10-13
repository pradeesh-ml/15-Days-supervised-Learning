# Credit Card Fraud Detection

This project demonstrates the use of XGBoost to detect credit card fraud. It includes data preprocessing, feature engineering, model training, and evaluation to accurately classify fraudulent transactions.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Results](#results)

## Introduction

The goal of this project is to detect fraudulent credit card transactions based on various transaction features. The project employs the XGBoost classifier to accurately classify transactions as fraudulent or legitimate. The model addresses class imbalance through downsampling techniques and evaluates performance using metrics such as precision, recall, and F1-score.

## Dataset

The dataset used in this project contains credit card transaction data, with features engineered through PCA (Principal Component Analysis) to ensure privacy and confidentiality.

### Features:

- **Time**: The number of seconds elapsed since the first transaction.
- **V1 - V28**: Principal components resulting from PCA applied to the original features, used to maintain data confidentiality.
- **Amount**: The transaction amount.
- **Class**: The target variable, indicating whether the transaction is fraudulent (1) or legitimate (0).

## Project Workflow

1. **Data Preprocessing**:
   - Load the dataset and perform initial data exploration.
   - Check for missing values and generate descriptive statistics.
   - Visualize class distribution and feature correlations.
   - Address class imbalance by downsampling the majority class to enhance model training.

2. **Exploratory Data Analysis (EDA)**:
   - Visualize the distribution of the target variable (Class).
   - Create a heatmap to understand correlations between features.

3. **Modeling**:
   - Split the dataset into training and testing sets.
   - Standardize the feature set using `StandardScaler`.
   - Train an XGBoost classifier on the training data.
   - Evaluate the model's performance using confusion matrix and classification report, capturing metrics such as precision, recall, F1-score, and accuracy.

4. **Visualization**:
   - Visualize the model's confusion matrix to assess its performance on the test set.

## Results

### Model Performance:
**Training Set**:
- **Precision**: 1.00
- **Recall**: 1.00
- **F1-Score**: 1.00
- **Accuracy**: 1.00

**Test Set**:
- **Precision**: 0.97 (Class 0), 0.92 (Class 1)
- **Recall**: 0.99 (Class 0), 0.86 (Class 1)
- **F1-Score**: 0.98 (Class 0), 0.89 (Class 1)
- **Accuracy**: 0.96

The model demonstrates excellent performance on both the training and test sets, achieving high precision and recall for both classes. This indicates a strong ability to detect fraudulent transactions while maintaining a low false positive rate. Further exploration of advanced techniques or additional feature engineering could enhance model robustness.
