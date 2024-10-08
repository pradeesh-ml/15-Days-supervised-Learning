# Customer Churn Prediction

This project demonstrates the use of K-Nearest Neighbors (KNN) to predict customer churn. It includes data preprocessing, feature engineering, hyperparameter tuning, and model evaluation to accurately classify customers who are likely to churn.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Results](#results)

## Introduction

The goal of this project is to predict customer churn based on various customer characteristics, including their demographic information, service usage, and payment methods. The project uses K-Nearest Neighbors (KNN) for classification, employing hyperparameter tuning via GridSearchCV to optimize model performance.

## Dataset

The dataset used in this project is from a telecommunications company and contains information about customer demographics, services, and churn status.

### Features:

- **gender**: Customer's gender.
- **SeniorCitizen**: Whether the customer is a senior citizen (1) or not (0).
- **Partner**: Whether the customer has a partner.
- **Dependents**: Whether the customer has dependents.
- **tenure**: Number of months the customer has stayed with the company.
- **PhoneService**: Whether the customer has phone service.
- **MultipleLines**: Whether the customer has multiple lines.
- **InternetService**: Type of internet service (DSL, Fiber optic, or None).
- **OnlineSecurity**: Whether the customer has online security.
- **OnlineBackup**: Whether the customer has online backup.
- **DeviceProtection**: Whether the customer has device protection.
- **TechSupport**: Whether the customer has tech support.
- **StreamingTV**: Whether the customer has streaming TV.
- **StreamingMovies**: Whether the customer has streaming movies.
- **Contract**: The type of customer contract (Month-to-month, One year, Two year).
- **PaperlessBilling**: Whether the customer uses paperless billing.
- **PaymentMethod**: The customer's payment method.
- **MonthlyCharges**: The monthly charge the customer pays.
- **TotalCharges**: The total charge accumulated over the customer's tenure.
- **Churn**: The target variable, indicating whether the customer churned (1) or stayed (0).

## Project Workflow

1. **Data Preprocessing**:
   - Handle missing values and correct data types (e.g., convert `TotalCharges` to numeric).
   - Remove unnecessary columns like `customerID` that do not contribute to prediction.
   - Label encode categorical variables for use in machine learning models.
   - Scale numeric features using MinMaxScaler.

2. **Exploratory Data Analysis (EDA)**:
   - Visualize the distribution of features such as `tenure`, `MonthlyCharges`, and `TotalCharges`.
   - Explore the relationship between customer churn and different categorical features using count plots.
   - Analyze the distribution of churned vs. non-churned customers across multiple services and contract types.

3. **Modeling**:
   - Split the data into training and testing sets.
   - Train a K-Nearest Neighbors (KNN) model on the training data.
   - Use GridSearchCV for hyperparameter tuning to find the optimal number of neighbors and distance metric.
   - Evaluate the model using a confusion matrix and classification report, including metrics like precision, recall, F1-score, and accuracy.

4. **Visualization**:
   - Plot the distribution of churned and non-churned customers for various features.
   - Visualize the model's confusion matrix to assess its performance on the test set.

## Results

### Model Performance:
**Training Set**:
- **Precision**: 1.00
- **Recall**: 1.00
- **F1-Score**: 1.00
- **Accuracy**: 1.00

**Test Set**:
- **Precision**: 0.79 (Class 0), 0.69 (Class 1)
- **Recall**: 0.95 (Class 0), 0.32 (Class 1)
- **F1-Score**: 0.86 (Class 0), 0.43 (Class 1)
- **Accuracy**: 0.78

The model performs well on the training set but shows some overfitting, as indicated by the performance drop on the test set, particularly in predicting customers who churn. Further model refinement or use of more advanced techniques could improve the test set performance.
