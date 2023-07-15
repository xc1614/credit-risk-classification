# Credit Risk Analysis Report

## Overview of the Analysis

The analysis involved using various techniques to train and evaluate a model for assessing loan risk. The dataset used was from a peer-to-peer lending services company and included historical lending activity. The goal was to build a model that could identify the creditworthiness of borrowers based on features such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt.

The total number of data points in the dataset was 77,536.

The analysis consisted of the following steps:

Data Split: The dataset was split into training and testing sets to evaluate the model's performance.

Initial Logistic Regression Model: An initial logistic regression model was created using the original data, with 75,036 low-risk data points and 2,500 high-risk data points. This model aimed to predict whether a loan to a borrower in the testing set would be classified as low risk or high risk.

Resampling with RandomOverSampler: The training data was resampled using the RandomOverSampler technique to address class imbalance. This ensured that both low-risk and high-risk labels had an equal number of data points, resulting in 56,277 data points for each class.

Logistic Regression Model with Resampled Data: A new logistic regression model was built using the resampled data. This model aimed to predict loan risk based on the resampled training data.

The purpose of these steps was to compare the performance of the initial logistic regression model trained on the original data with the performance of the logistic regression model trained on the resampled data. This comparison would help assess the effectiveness of resampling in addressing class imbalance and improving the model's ability to predict loan risk.

 ## Results:

Logistic Regression Model 1:

Precision for label "0": 1.00
Precision for label "1": 0.87
Recall for label "0": 1.00
Recall for label "1": 0.89
F1-score for label "0": 1.00
F1-score for label "1": 0.88
Accuracy: 0.99

Logistic Regression Model 2:

Precision for label "0": 1.00
Precision for label "1": 0.87
Recall for label "0": 1.00
Recall for label "1": 1.00
F1-score for label "0": 1.00
F1-score for label "1": 0.93
Accuracy: 1.00

## Summary

Logistic Regression Model 2 demonstrates slightly better performance for the high-risk loan label, achieving perfect recall and a higher F1-score, while both models perform equally well for the healthy loan label. Logistic Regression Model 2 also has a slightly higher overall accuracy. Therefore, Logistic Regression Model 2 can be considered the better-performing model in this comparison.