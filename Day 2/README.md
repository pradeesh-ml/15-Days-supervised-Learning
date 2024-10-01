# Car Price Prediction Model

This project demonstrates the use of various regression techniques to predict car prices based on a dataset containing various features related to cars. The primary models used are **Ridge Regression**, **Lasso Regression**, and **Random Forest Regressor**.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction
In this project, we aim to predict the **Price** of cars based on features such as engine volume, mileage, fuel type, and more. The project involves data preprocessing, feature engineering, model training, and evaluation. Due to the poor performance of Ridge and Lasso regression, we implement a Random Forest Regressor for better accuracy.

## Dataset
The dataset used in this project is `car_price_prediction.csv`, which contains various features related to cars. The dataset consists of multiple observations on various features, including:

### Features:
- **Price**: The target variable representing the price of the car.
- **Levy**: Additional fees or levies associated with the car.
- **Manufacturer**: The manufacturer of the car.
- **Model**: The specific model of the car.
- **Prod. year**: The year the car was produced.
- **Category**: The category or type of the car (e.g., sedan, SUV).
- **Leather interior**: Indicates whether the car has a leather interior (Yes/No).
- **Fuel type**: The type of fuel the car uses (e.g., petrol, diesel).
- **Engine volume**: The engine capacity of the car.
- **Mileage**: The distance the car can travel per unit of fuel.
- **Cylinders**: The number of cylinders in the car's engine.
- **Gear box type**: The type of gearbox (e.g., automatic, manual).
- **Drive wheels**: The type of drive (e.g., front-wheel, rear-wheel).
- **Doors**: The number of doors on the car.
- **Wheel**: The type of wheel (e.g., alloy, steel).
- **Color**: The color of the car.
- **Airbags**: The number of airbags in the car.

## Project Workflow

1. **Data Preprocessing**:
   - Load the dataset and display basic information.
   - Handle invalid values and convert types as necessary.
   - Visualize the distribution of the target variable (Price).
   - Perform outlier detection and removal using the Interquartile Range (IQR) method.
   - Encode categorical features using Label Encoding.

2. **Modeling**:
   - Split the data into training and test sets.
   - Train **Ridge Regression** and **Lasso Regression** models.
   - Evaluate the models using **Mean Squared Error (MSE)** and **R-squared (R²)** metrics.
   - Train a **Random Forest Regressor** for improved performance.

## Results

The performance of the models is evaluated using the following metrics:

- **Ridge Regression**:
  - Mean Squared Error: 97,932,851.11
  - R² Score: 0.23

- **Lasso Regression**:
  - Mean Squared Error: 97,934,021.70
  - R² Score: 0.23

- **Random Forest Regressor**:
  - Mean Squared Error: 27,109,018.52
  - R² Score: 0.78

The **Random Forest Regressor** demonstrated significantly better performance compared to both **Ridge** and **Lasso regression** models.


