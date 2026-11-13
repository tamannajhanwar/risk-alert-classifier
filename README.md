# Risk Alert Classification

## Project Overview

This project focuses on building and evaluating machine learning classification models to identify customers based on their risk status. The main objective is to predict whether a customer belongs to the **High Risk** or **Low Risk** category using different classification algorithms.

The project explores data preprocessing, handling imbalanced datasets, model implementation, performance evaluation, and hyperparameter optimization.

## Problem Statement

The objective is to develop a machine learning model that accurately classifies customers into different risk categories. Since identifying high-risk customers is important, special attention is given to minimizing false negatives and improving recall for the minority class.

## Dataset Description

- **Dataset Name:** Risk Alert Classifier Dataset
- **Number of Records:** 4,600
- **Target Variable:** `risk_status`
- **Target Classes:** High Risk and Low Risk

The dataset contains customer-related information used to predict their risk status.

## Technologies and Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn

## Project Workflow

### 1. Data Preprocessing

- Loaded and explored the dataset.
- Checked missing values and duplicate records.
- Separated independent and dependent variables.
- Removed unnecessary columns.
- Applied train-test splitting.
- Used KNN Imputation for numerical missing values.
- Applied appropriate encoding and scaling techniques.

### 2. Logistic Regression

Implemented Logistic Regression as the baseline classification model.

Evaluated the model using:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Type I and Type II Errors

### 3. Handling Imbalanced Data

Since the dataset contains an imbalanced target variable, different balancing techniques were implemented:

- Class Weighting
- Random Undersampling
- Random Oversampling
- SMOTE
- ADASYN

The performance of these techniques was compared using Recall, F1 Score, and ROC-AUC.

### 4. Decision Tree Classifier

Implemented a Decision Tree Classifier to classify customers based on their risk status.

- Trained the Decision Tree model.
- Evaluated training and testing performance.
- Analyzed overfitting by comparing training and testing accuracy.

### 5. Random Forest Classifier

Implemented Random Forest Classifier to improve prediction performance and generalization.

Compared Decision Tree and Random Forest based on:
- Accuracy
- Training Performance
- Testing Performance
- Generalization Ability

### 6. Hyperparameter Optimization

Applied hyperparameter tuning to improve model performance.

Techniques used:

- RandomizedSearchCV
- GridSearchCV

Optimized hyperparameters for:
- Decision Tree Classifier
- Random Forest Classifier

### 7. Model Evaluation

Evaluated and compared different classification models using:

- Accuracy Score
- Precision Score
- Recall Score
- F1 Score
- Confusion Matrix
- ROC Curve
- ROC-AUC Score
- False Negative Count

## Models Implemented

1. Logistic Regression
2. Logistic Regression with Class Weighting
3. Logistic Regression with Undersampling
4. Logistic Regression with Oversampling
5. Logistic Regression with SMOTE
6. Logistic Regression with ADASYN
7. Decision Tree Classifier
8. Random Forest Classifier
9. Hyperparameter-Tuned Decision Tree
10. Hyperparameter-Tuned Random Forest

## Key Findings

- The dataset contains an imbalance between High Risk and Low Risk customers.
- Logistic Regression achieved strong baseline performance.
- Different sampling techniques were tested to handle class imbalance.
- Decision Tree and Random Forest were compared to analyze overfitting and generalization.
- Random Forest demonstrated better generalization than the untuned Decision Tree in the notebook's comparison.
- Randomized Search CV and Grid Search CV were used to optimize model hyperparameters.
- Logistic Regression was selected as the preferred model based on the notebook's final evaluation, particularly its zero false negatives.

## Conclusion

This project demonstrates the complete machine learning classification process, starting from data preprocessing and handling class imbalance to model implementation, evaluation, and hyperparameter tuning.

Different classification algorithms were explored and compared to identify a suitable model for customer risk prediction. The main focus was on improving classification performance while minimizing false negatives to ensure better identification of high-risk customers.

**Dataset:** Risk_Alert_Classifier_Dataset_4600.csv

**Notebook:** pr3.ipynb
