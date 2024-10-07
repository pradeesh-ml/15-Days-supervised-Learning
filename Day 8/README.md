# Email Spam Prediction

This project demonstrates the use of Logistic Regression to predict whether an email is spam or not, based on its textual content. It includes data preprocessing, text vectorization using TF-IDF, and model evaluation.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Results](#results)

## Introduction

The goal of this project is to classify emails as either spam or ham (non-spam) using logistic regression. The model utilizes TF-IDF (Term Frequency-Inverse Document Frequency) for text vectorization and applies logistic regression for classification. The project covers data cleaning, text preprocessing, and model evaluation to achieve a high-performance spam detection system.

## Dataset

The dataset used in this project contains email data labeled as either spam or ham.

### Features:

- **text**: The email's textual content.
- **spam**: The target variable, indicating whether the email is spam (1) or ham (0).

## Project Workflow

1. **Data Preprocessing**:
   - Load the dataset and check for missing values and duplicates.
   - Remove duplicate records to ensure data integrity.
   - Apply basic text cleaning, such as removing the 'Subject:' prefix from the email content.
   - Balance the dataset by undersampling the majority class (ham) to match the number of spam emails.

2. **Feature Engineering**:
   - Use TF-IDF vectorization to transform the textual content into numerical features for modeling.

3. **Modeling**:
   - Split the dataset into training and testing sets.
   - Train a Logistic Regression model on the training data.
   - Evaluate the model on the test data using a confusion matrix and classification report, including metrics like precision, recall, F1-score, and accuracy.

4. **Visualization**:
   - Plot the distribution of spam vs. ham emails before and after undersampling.
   - Visualize the confusion matrix to assess the model’s performance.

## Results

### Model Performance:
- **Precision**: 0.98
- **Recall**: 0.98
- **F1-Score**: 0.98
- **Accuracy**: 0.98

The logistic regression model demonstrates strong performance, with high accuracy and balanced precision and recall scores, making it highly effective at distinguishing between spam and ham emails.
