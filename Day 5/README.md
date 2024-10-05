# Concrete Strength Prediction

This project demonstrates the use of a Random Forest Regressor to predict the compressive strength of concrete based on various input features. It includes data preprocessing, outlier handling, feature visualization, hyperparameter tuning using RandomizedSearchCV, and model evaluation.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Results](#results)

## Introduction

In this project, we aim to predict the compressive strength of concrete based on factors like the proportions of various ingredients and the age of the concrete. The project leverages a Random Forest Regressor to model the relationships in the data, following essential steps in data preprocessing, outlier treatment, and hyperparameter tuning.

## Dataset

The dataset used in this project contains data on concrete mixtures and their corresponding strength. It consists of multiple features that describe the proportions of various components used in concrete production.

### Features:

- **Cement**: Amount of cement in the mixture
- **Blast Furnace Slag**: Amount of blast furnace slag in the mixture
- **Fly Ash**: Amount of fly ash in the mixture
- **Water**: Amount of water in the mixture
- **Superplasticizer**: Amount of superplasticizer in the mixture
- **Coarse Aggregate**: Amount of coarse aggregate in the mixture
- **Fine Aggregate**: Amount of fine aggregate in the mixture
- **Age**: Age of the concrete (in days)
- **Strength**: Compressive strength of the concrete (Target)

## Project Workflow

1. **Data Preprocessing**:
   - Load the dataset and check for data integrity.
   - Explore the dataset using summary statistics and visualizations (e.g., histograms and boxplots).
   - Identify and handle outliers by replacing them with the mean of their respective columns.
   - Visualize correlations among features using a heatmap.

2. **Modeling**:
   - Split the dataset into training and testing sets.
   - Use a Random Forest Regressor model for predictions.
   - Tune hyperparameters such as `n_estimators`, `max_depth`, and `max_features` using RandomizedSearchCV.
   - Train the model and evaluate its performance using metrics like Mean Squared Error (MSE) and R-squared (R²) score.

3. **Visualization**:
   - Correlation heatmap to show feature relationships.
   - Scatter plots to visualize actual vs. predicted compressive strength.
   - Boxplots to display the distribution of features post outlier treatment.

## Results

### Training Set Performance:
- **Mean Squared Error (MSE)**: 5.43
- **R² Score**: 0.98

### Test Set Performance:
- **Mean Squared Error (MSE)**: 5.43
- **R² Score**: 0.82
