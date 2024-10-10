# Iris Flower Classification

This project demonstrates the use of a Decision Tree Classifier to classify iris flowers based on their features. It includes data preprocessing, exploratory data analysis (EDA), model training, and evaluation to accurately predict the species of iris flowers.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Results](#results)

## Introduction

The goal of this project is to classify iris flowers into three species based on their morphological characteristics. The dataset contains measurements of sepal length, sepal width, petal length, and petal width, which are used as features for classification. A Decision Tree Classifier is employed to create a predictive model, with evaluation metrics to assess its performance.

## Dataset

The dataset used in this project is the well-known Iris dataset, which contains measurements of iris flowers from three different species.

### Features:

- **sepal_length**: Length of the sepal (cm).
- **sepal_width**: Width of the sepal (cm).
- **petal_length**: Length of the petal (cm).
- **petal_width**: Width of the petal (cm).
- **species**: The target variable indicating the species of the iris flower (Iris-setosa, Iris-versicolor, Iris-virginica).

## Project Workflow

1. **Data Preprocessing**:
   - Load the dataset and display its basic information.
   - Check for missing values and handle them if necessary.
   - Visualize the distribution of iris species.

2. **Exploratory Data Analysis (EDA)**:
   - Visualize the distributions of features such as `sepal_length`, `sepal_width`, `petal_length`, and `petal_width`.
   - Use pairplots to analyze the relationships between different features and the species.

3. **Modeling**:
   - Split the data into training and testing sets.
   - Train a Decision Tree Classifier on the training data.
   - Evaluate the model using confusion matrix and classification report to obtain precision, recall, F1-score, and accuracy.

## Results

### Model Performance:
**Training Set**:
- **Precision**: 1.00 (Iris-setosa), 1.00 (Iris-versicolor), 1.00 (Iris-virginica)
- **Recall**: 1.00 (Iris-setosa), 1.00 (Iris-versicolor), 1.00 (Iris-virginica)
- **F1-Score**: 1.00 (Iris-setosa), 1.00 (Iris-versicolor), 1.00 (Iris-virginica)
- **Accuracy**: 1.00

**Test Set**:
- **Precision**: 1.00 (Iris-setosa), 1.00 (Iris-versicolor), 1.00 (Iris-virginica)
- **Recall**: 1.00 (Iris-setosa), 1.00 (Iris-versicolor), 1.00 (Iris-virginica)
- **F1-Score**: 1.00 (Iris-setosa), 1.00 (Iris-versicolor), 1.00 (Iris-virginica)
- **Accuracy**: 1.00

The model demonstrates perfect classification performance on both the training and test sets, indicating that it accurately predicts the species of iris flowers based on their morphological features. Further exploration with different algorithms or hyperparameter tuning may enhance the model's robustness.
