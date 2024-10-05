# Energy Efficiency Prediction

This project demonstrates the use of Support Vector Regression (SVR) to predict the heating and cooling loads of a building based on various input features. It includes data preprocessing, feature visualization, hyperparameter tuning using RandomizedSearchCV, and model evaluation.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Results](#results)

## Introduction

In this project, we aim to predict the heating and cooling loads of a building based on various factors, such as the building's dimensions, orientation, and glazing areas. The project leverages Support Vector Regression to model the relationships in the data, following essential steps in data preprocessing, feature visualization, and hyperparameter tuning.

## Dataset

The dataset used in this project contains data on energy efficiency in buildings and their corresponding heating and cooling loads. It consists of multiple features that describe the physical characteristics of the buildings.

### Features:

- **Relative_Compactness**: The compactness of the building
- **Surface_Area**: The surface area of the building
- **Wall_Area**: The total wall area of the building
- **Roof_Area**: The total roof area of the building
- **Overall_Height**: The overall height of the building
- **Orientation**: The orientation of the building (e.g., North, South)
- **Glazing_Area**: The area of glazing in the building
- **Glazing_Area_Distribution**: The distribution of the glazing area across the building
- **Heating_Load**: The target variable representing the heating load of the building
- **Cooling_Load**: The target variable representing the cooling load of the building

## Project Workflow

1. **Data Preprocessing**:
   - Load the dataset and check for data integrity.
   - Explore the dataset using summary statistics and visualizations (e.g., histograms and scatter plots).
   - Check for missing values and handle them appropriately.
   - Scale the features using StandardScaler for better model performance.

2. **Modeling**:
   - Split the dataset into training and testing sets.
   - Use a Support Vector Regressor (SVR) model for predictions of both heating and cooling loads.
   - Tune hyperparameters such as `C`, `epsilon`, and `kernel` using RandomizedSearchCV.
   - Train the model and evaluate its performance using metrics like Mean Squared Error (MSE) and R-squared (R²) score.

3. **Visualization**:
   - Correlation heatmap to show feature relationships.

## Results

### Heating Load Performance:
- **Mean Squared Error (MSE)**: 0.3176
- **R² Score**: 0.9969

### Cooling Load Performance:
- **Mean Squared Error (MSE)**: 2.1262
- **R² Score**: 0.9764
