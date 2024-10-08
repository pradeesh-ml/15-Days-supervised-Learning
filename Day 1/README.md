# Boston Housing Price Prediction

This project demonstrates the use of **Linear Regression** to predict the median value of owner-occupied homes in the Boston area using the Boston Housing Dataset. It involves data preprocessing, feature engineering, model training, and evaluation.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction
In this project, we aim to predict the **Median Value of Homes (MEDV)** based on various features such as crime rate, property tax rate, number of rooms, etc. We use a **Linear Regression** model with basic preprocessing steps, including handling missing values, feature scaling, and dealing with multicollinearity.

## Dataset
The dataset used in this project is the Boston Housing Dataset, which contains information collected by the U.S Census Service concerning housing in the area of Boston, Massachusetts. The dataset consists of 506 observations on 13 features and a target variable `MEDV` (median home value).

### Features:
- **CRIM**: Per capita crime rate by town
- **ZN**: Proportion of residential land zoned for lots over 25,000 sq. ft.
- **INDUS**: Proportion of non-retail business acres per town
- **CHAS**: Charles River dummy variable (1 if tract bounds river; 0 otherwise)
- **NOX**: Nitrogen oxide concentration (parts per 10 million)
- **RM**: Average number of rooms per dwelling
- **AGE**: Proportion of owner-occupied units built before 1940
- **DIS**: Weighted distances to five Boston employment centers
- **RAD**: Index of accessibility to radial highways
- **TAX**: Full-value property tax rate per $10,000
- **PTRATIO**: Pupil-teacher ratio by town
- **B**: Proportion of black residents by town
- **LSTAT**: Percentage of lower-status population
- **MEDV**: Median value of owner-occupied homes (Target)

## Project Workflow

1. **Data Preprocessing**:
   - Handle missing values using mean or mode imputation.
   - Visualize correlations between features.
   - Remove multicollinear features (e.g., `RAD`).
   - Visualize the distribution of the target variable (`MEDV`).

2. **Modeling**:
   - Split the data into training and test sets.
   - Train a **Linear Regression** model.
   - Evaluate the model using **Mean Squared Error (MSE)** and **R-squared (R²)** metrics.

3. **Visualization**:
   - Correlation heatmap for feature relationships.
   - Distribution plot for the target variable.
   - Scatter plot for predicted vs actual values.

