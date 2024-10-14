# Sentiment Analysis on Tweets

This project demonstrates the use of Naive Bayes to perform sentiment analysis on a dataset of tweets. It includes data preprocessing, feature extraction using TF-IDF, model training, evaluation, and visualization of results.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Results](#results)

## Introduction

The goal of this project is to analyze the sentiment of tweets and classify them as positive or negative. The project utilizes the Naive Bayes algorithm for classification and includes steps for data cleaning, tokenization, stop word removal, and feature extraction through TF-IDF.

## Dataset

The dataset used in this project consists of tweets with their sentiment labels. The columns in the dataset are:

- **target**: Sentiment label (1 for positive, 0 for negative).
- **ids**: Unique identifier for each tweet.
- **date**: Timestamp of the tweet.
- **flag**: Additional metadata (not used in analysis).
- **user**: Username of the tweet author.
- **text**: The actual tweet text.

**Dataset Link**: https://www.kaggle.com/datasets/kazanova/sentiment140

## Project Workflow

1. **Data Preprocessing**:
   - Load the dataset and drop unnecessary columns.
   - Clean the text data by removing URLs, mentions, punctuation, and stop words.
   - Convert text to lowercase and handle multiple spaces.
   - Tokenize the text to prepare for feature extraction.

2. **Exploratory Data Analysis (EDA)**:
   - Visualize the distribution of sentiment labels using count plots.
   - Create word clouds for positive and negative tweets to analyze common terms.

3. **Modeling**:
   - Split the data into training and testing sets.
   - Use TF-IDF to transform the text data into feature vectors.
   - Train a Naive Bayes classifier on the training data.
   - Evaluate the model's performance using confusion matrices and classification reports.

4. **Visualization**:
   - Display the confusion matrix to assess the model's performance.
   - Plot the ROC curve to visualize the trade-off between true positive and false positive rates.

## Results

### Model Performance:

**Training Set**:
- **Precision**: 0.80
- **Recall**: 0.80
- **F1-Score**: 0.80
- **Accuracy**: 0.80

**Test Set**:
- **Precision**: 0.76 (Class 0), 0.77 (Class 1)
- **Recall**: 0.78 (Class 0), 0.75 (Class 1)
- **F1-Score**: 0.77 (Class 0), 0.76 (Class 1)
- **Accuracy**: 0.76

The model shows consistent performance across the training and test sets, indicating a balanced classification of sentiment. However, there may be opportunities to improve accuracy further through additional feature engineering or model tuning.
