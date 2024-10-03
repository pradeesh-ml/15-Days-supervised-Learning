# Bike Sharing Demand Prediction

This project demonstrates the use of a Decision Tree Regressor to predict bike-sharing demand based on various environmental and temporal factors. It includes data preprocessing, feature engineering, hyperparameter tuning using GridSearchCV, and model evaluation.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Results](#results)

## Introduction

In this project, we aim to predict the demand for bike-sharing services based on factors like temperature, humidity, weather conditions, and the time of day. The project leverages a Decision Tree Regressor to capture complex relationships in the data, following essential steps in data preprocessing, feature extraction, and hyperparameter tuning.

## Dataset

The dataset used in this project contains data on bike rentals and several factors that could influence bike-sharing demand. It consists of multiple features recorded at hourly intervals, such as weather conditions, time, and environmental variables.

### Features:

- **season**: Season of the year (1: Winter, 2: Spring, 3: Summer, 4: Fall)
- **holiday**: Whether the day is a holiday (0: No, 1: Yes)
- **workingday**: Whether the day is a working day (0: No, 1: Yes)
- **weather**: Weather conditions (1: Clear, 2: Mist, 3: Light Snow/Rain, 4: Heavy Rain)
- **temp**: Temperature (in Celsius)
- **humidity**: Humidity level
- **windspeed**: Wind speed
- **count**: Number of bikes rented (Target)
- **Day**: Day of the month
- **Year**: Year of the data entry
- **Hour**: Hour of the day

## Project Workflow

1. **Data Preprocessing**:
   - Handle missing values and check for data integrity.
   - Convert the `datetime` column into useful features like Day, Year, and Hour.
   - Drop irrelevant or highly correlated columns (e.g., `casual`, `registered`, `Month`).
   - Visualize data using bar plots and heatmaps to understand feature relationships.

2. **Modeling**:
   - Split the dataset into training and testing sets.
   - Use a Decision Tree Regressor model for predictions.
   - Tune hyperparameters such as `max_depth`, `min_samples_split`, and `criterion` using GridSearchCV.
   - Train the model and evaluate its performance using metrics like Root Mean Squared Error (RMSE) and R-squared (R²) score.

3. **Visualization**:
   - Correlation heatmap to show feature relationships.
   - Bar plots to display demand trends over time and across different weather conditions.
   - Scatter plot for actual vs predicted bike-sharing demand.

## Results

### Training Set Performance:
- **Root Mean Squared Error (RMSE)**: 41.29
- **R² Score**: 0.95

### Test Set Performance:
- **Root Mean Squared Error (RMSE)**: 54.92
- **R² Score**: 0.91
