# Wine Quality Prediction

This project demonstrates the use of a Decision Tree Classifier to predict wine quality. The dataset includes various chemical properties of wines, and the goal is to classify wines as good or bad based on their quality score. The project covers data preprocessing, exploratory data analysis (EDA), model training, and evaluation.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Results](#results)

## Introduction

The objective of this project is to predict wine quality using a Decision Tree Classifier. The wine quality is determined by various chemical properties like acidity, sulfur dioxide content, alcohol levels, etc. The target variable, `quality`, is binarized to classify wines as either good (1) or bad (0) based on their score.

## Dataset

The dataset used in this project contains data on different chemical attributes of wines and their corresponding quality scores.

### Features:

- **fixed acidity**: Fixed acidity level.
- **volatile acidity**: Volatile acidity level.
- **citric acid**: Citric acid content.
- **residual sugar**: Amount of residual sugar.
- **chlorides**: Chloride content.
- **free sulfur dioxide**: Free sulfur dioxide content.
- **total sulfur dioxide**: Total sulfur dioxide content.
- **density**: Density of the wine.
- **pH**: pH value of the wine.
- **sulphates**: Sulphate content.
- **alcohol**: Alcohol content.
- **quality**: Wine quality score (used as the target variable, binarized for classification).

## Project Workflow

1. **Data Preprocessing**:
   - Load the dataset and inspect the structure.
   - Drop the irrelevant `Id` column.
   - Convert the `quality` column into a binary classification (good = 1, bad = 0).
   - Split the dataset into features (`X`) and target (`y`).
   - Scale the feature values using StandardScaler to normalize the data.

2. **Exploratory Data Analysis (EDA)**:
   - Visualize the distribution of each feature using histograms.
   - Plot the correlation heatmap to understand relationships between features.
   - Analyze the distribution of wine quality using count plots.

3. **Modeling**:
   - Train a Decision Tree Classifier using training data.
   - Hyperparameters include `criterion='entropy'`, `max_depth=15`, `min_samples_split=16`, and `min_samples_leaf=19`.
   - Evaluate the model on both the training and test sets using classification reports and confusion matrices.

4. **Model Evaluation**:
   - Display confusion matrices for both training and test sets.
   - Plot the ROC curve to visualize model performance.
   - Calculate AUC to assess the quality of the classifier.

## Results

### Model Performance:

**Training Set**:
- **Precision (Class 0)**: 0.79
- **Recall (Class 0)**: 0.75
- **F1-Score (Class 0)**: 0.77
- **Precision (Class 1)**: 0.80
- **Recall (Class 1)**: 0.83
- **F1-Score (Class 1)**: 0.82
- **Accuracy**: 0.80

**Test Set**:
- **Precision (Class 0)**: 0.72
- **Recall (Class 0)**: 0.68
- **F1-Score (Class 0)**: 0.70
- **Precision (Class 1)**: 0.73
- **Recall (Class 1)**: 0.77
- **F1-Score (Class 1)**: 0.75
- **Accuracy**: 0.73


## Conclusion

This project illustrates how a Decision Tree Classifier can be used to predict wine quality based on chemical properties. The model demonstrates reasonable performance but could be enhanced with more advanced techniques or further tuning. Visualization techniques like ROC curves and confusion matrices provide a clear understanding of the model's effectiveness.
