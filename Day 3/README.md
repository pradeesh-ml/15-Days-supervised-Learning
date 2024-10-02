# Medical Insurance Cost Prediction

This project demonstrates the use of Polynomial Regression to predict medical insurance costs using various personal and demographic factors. It involves data preprocessing, feature engineering, model training, and evaluation.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Results](#results)

## Introduction

In this project, we aim to predict the cost of medical insurance based on various features such as age, BMI, smoking status, and more. The project uses a Polynomial Regression model and involves essential preprocessing steps such as encoding categorical variables, scaling numerical features, and feature engineering to capture non-linear relationships.

## Dataset

The dataset used in this project is the Medical Insurance Dataset, which contains information related to insurance costs and several factors that affect these costs. It consists of 1338 observations on 7 features and a target variable, `charges` (the cost of insurance).

### Features:

- **age**: Age of the policyholder
- **sex**: Gender of the policyholder
- **bmi**: Body mass index, a measure of body fat based on height and weight
- **children**: Number of children/dependents covered by the insurance
- **smoker**: Whether the policyholder smokes or not (Yes/No)
- **region**: The region where the policyholder resides
- **charges**: The actual insurance cost (Target)

## Project Workflow

1. **Data Preprocessing**:
   - Handle missing values (if any).
   - Encode categorical variables (sex, smoker, region) using Label Encoding.
   - Scale numerical features (age, bmi) using StandardScaler.
   - Visualize feature distributions and their relationship with the target variable.

2. **Modeling**:
   - Split the dataset into training and test sets.
   - Apply Polynomial Features transformation to create non-linear relationships.
   - Train a Polynomial Regression model.
   - Evaluate the model using metrics like Mean Squared Error (MSE) and R-squared (R²) score.

3. **Visualization**:
   - Correlation heatmap between features.
   - Distribution plots for key numerical features.
   - Scatter plot for actual vs predicted insurance charges.

## Results

### Training Set Performance:
- **Mean Squared Error**: 23,665,891
- **R² Score**: 0.84

### Test Set Performance:
- **Mean Squared Error**: 19,976,725
- **R² Score**: 0.86

