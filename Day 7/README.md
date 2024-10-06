# Retail Sales Prediction

This project demonstrates the use of XGBoost regression to predict the total sales amount based on various input features. It includes data preprocessing, feature visualization, hyperparameter tuning using RandomizedSearchCV, and model evaluation.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Results](#results)

## Introduction

In this project, we aim to predict the total sales amount of retail transactions based on various factors such as product category, customer demographics, and transaction details. The project leverages XGBoost regression to model the relationships in the data, following essential steps in data preprocessing, feature visualization, and hyperparameter tuning.

## Dataset

The dataset used in this project contains data on retail transactions and their corresponding sales amounts. It consists of multiple features that describe the details of each transaction.

### Features:

- **Gender**: The gender of the customer (e.g., Male, Female)
- **Age**: The age of the customer
- **Product Category**: The category of the product sold
- **Quantity**: The quantity of the product purchased
- **Price per Unit**: The price of each unit of the product
- **Total Amount**: The target variable representing the total sales amount for the transaction

## Project Workflow

1. **Data Preprocessing**:
   - Load the dataset and check for data integrity.
   - Explore the dataset using summary statistics and visualizations (e.g., bar plots for product category).
   - Check for missing values and handle them appropriately.
   - Convert categorical features into numerical representations using Label Encoding.

2. **Modeling**:
   - Split the dataset into training and testing sets.
   - Use an XGBoost regressor model for predictions of total sales amount.
   - Tune hyperparameters such as `n_estimators`, `learning_rate`, and `max_depth` using RandomizedSearchCV.
   - Train the model and evaluate its performance using metrics like Mean Squared Error (MSE) and R-squared (R²) score.

3. **Visualization**:
   - Visualize the relationships between features and total sales using bar plots and scatter plots.
   - Plot the predicted vs. actual total sales to assess model performance.

## Results

### Model Performance:
- **Training Set Performance**:
  - **Mean Squared Error (MSE)**: 2.9293e-08
  - **R² Score**: 0.9999999999999106

- **Test Set Performance**:
  - **Mean Squared Error (MSE)**: 2.9626e-08
  - **R² Score**: 0.999999999999894
