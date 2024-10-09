# Breast Cancer Prediction

This project demonstrates the use of a Support Vector Machine (SVM) to predict breast cancer. It includes data preprocessing, feature selection, and model evaluation to accurately classify whether a tumor is malignant or benign.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Results](#results)

## Introduction

The goal of this project is to predict whether a breast tumor is malignant (cancerous) or benign (non-cancerous) based on various tumor characteristics. The project employs a Support Vector Machine (SVM) classifier to make predictions after optimizing the model's performance using data preprocessing and feature selection techniques.

## Dataset

The dataset used in this project contains various measurements and characteristics of breast tumors. It includes information such as the size, texture, and smoothness of tumors, with a target label indicating whether the tumor is malignant or benign.

### Features:

- **radius_mean**: Mean of distances from center to points on the perimeter.
- **texture_mean**: Standard deviation of gray-scale values.
- **perimeter_mean**: Mean size of the core tumor.
- **area_mean**: Mean area of the tumor.
- **smoothness_mean**: Local variation in radius lengths.
- **compactness_mean**: Perimeter² / area - 1.0.
- **concavity_mean**: Severity of concave portions of the contour.
- **concave points_mean**: Number of concave portions of the contour.
- **symmetry_mean**: Symmetry of the tumor.
- **fractal_dimension_mean**: "Coastline approximation" - 1.
- And various other measurements related to the tumor’s size, shape, and texture.

The target variable is:
- **diagnosis**: The diagnosis of the tumor, where 1 represents malignant and 0 represents benign.

## Project Workflow

1. **Data Preprocessing**:
   - Remove irrelevant columns like `id` and handle missing values (if any).
   - Encode the target variable (`diagnosis`), where malignant (M) is encoded as 1, and benign (B) is encoded as 0.
   - Standardize the feature set using `StandardScaler` to ensure all features have the same scale.

2. **Exploratory Data Analysis (EDA)**:
   - Visualize correlations between features using a heatmap.
   - Identify highly correlated features and remove them to prevent multicollinearity.
   - Explore the distribution of malignant and benign tumors across various features.

3. **Feature Selection**:
   - Calculate the correlation matrix to detect highly correlated features (correlation > 0.90).
   - Drop features that are highly correlated to improve model performance and reduce overfitting.

4. **Modeling**:
   - Split the dataset into training and testing sets.
   - Train a Support Vector Machine (SVM) classifier on the training data.
   - Evaluate the model using the confusion matrix and classification report, analyzing metrics such as precision, recall, F1-score, and accuracy.

## Results

### Model Performance:
**Training Set**:
- **Precision**: 0.98 (Class 0), 1.00 (Class 1)
- **Recall**: 1.00 (Class 0), 0.96 (Class 1)
- **F1-Score**: 0.99 (Class 0), 0.98 (Class 1)
- **Accuracy**: 0.98

**Test Set**:
- **Precision**: 0.94 (Class 0), 0.93 (Class 1)
- **Recall**: 0.96 (Class 0), 0.91 (Class 1)
- **F1-Score**: 0.95 (Class 0), 0.92 (Class 1)
- **Accuracy**: 0.94

The model performs exceptionally well on both the training and test sets, achieving high accuracy and precision. The balanced performance indicates that the SVM model generalizes well to unseen data, making it a robust classifier for predicting breast cancer.
