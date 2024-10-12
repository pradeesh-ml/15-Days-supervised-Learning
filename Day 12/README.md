# Loan Default Prediction

This project demonstrates the use of a Random Forest Classifier to predict loan defaults. It includes data preprocessing, feature engineering, class imbalance handling, and model evaluation to classify whether a borrower is likely to default on a loan.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Results](#results)

## Introduction

The goal of this project is to predict loan defaults based on various borrower characteristics, such as demographic information, loan details, and credit history. The project uses a Random Forest Classifier to perform classification and addresses class imbalance by upsampling the minority class.

## Dataset

The dataset used in this project contains borrower demographic information, loan-related features, and the target variable `Default` (indicating if a borrower defaulted or not).

### Features:

- **LoanID**: Unique identifier for each loan (removed for modeling).
- **Age**: Age of the borrower.
- **Income**: Monthly income of the borrower.
- **LoanAmount**: Amount of the loan.
- **CreditScore**: Credit score of the borrower.
- **MonthsEmployed**: Number of months the borrower has been employed.
- **NumCreditLines**: Number of open credit lines.
- **InterestRate**: Interest rate on the loan.
- **LoanTerm**: Loan repayment term in months.
- **DTIRatio**: Debt-to-income ratio.
- **Education**: Education level of the borrower.
- **EmploymentType**: Type of employment (e.g., salaried, self-employed).
- **MaritalStatus**: Marital status of the borrower.
- **HasMortgage**: Whether the borrower has a mortgage (binary).
- **HasDependents**: Whether the borrower has dependents (binary).
- **LoanPurpose**: Purpose of the loan (e.g., home, education, personal).
- **HasCoSigner**: Whether the borrower has a co-signer (binary).
- **Default**: Target variable indicating loan default (1) or non-default (0).

## Project Workflow

1. **Data Preprocessing**:
   - Removed unnecessary columns like `LoanID`.
   - Encoded binary categorical variables using `LabelEncoder` and one-hot encoded other categorical variables.
   - Scaled numerical features using `StandardScaler` to ensure uniformity in magnitude.

2. **Exploratory Data Analysis (EDA)**:
   - Visualized the distribution of the target variable `Default`.
   - Examined the relationship between numerical features (e.g., `Income`, `CreditScore`) and loan default status using box plots.
   
3. **Handling Class Imbalance**:
   - Addressed class imbalance by upsampling the minority class (`Default=1`).

4. **Modeling**:
   - Split the data into training and testing sets.
   - Trained a Random Forest Classifier on the training data.
   - Evaluated the model using a confusion matrix, classification report, and metrics such as precision, recall, F1-score, and accuracy.

5. **Visualization**:
   - Plotted the distribution of loan defaults across various features.
   - Visualized the confusion matrix to assess model performance on the test set.

## Results

### Model Performance:
**Training Set**:
- **Precision**: 1.00 (Class 0), 1.00 (Class 1)
- **Recall**: 1.00 (Class 0), 1.00 (Class 1)
- **F1-Score**: 1.00 (Class 0), 1.00 (Class 1)
- **Accuracy**: 1.00

**Test Set**:
- **Precision**: 1.00 (Class 0), 0.98 (Class 1)
- **Recall**: 0.98 (Class 0), 1.00 (Class 1)
- **F1-Score**: 0.99 (Class 0), 0.99 (Class 1)
- **Accuracy**: 0.99

The model performs excellently on both the training and test sets, with near-perfect precision, recall, and F1-scores. This high performance, particularly on the test set, indicates that the model generalizes well to unseen data.
