# credit-risk-classification
A supervised learning exercise

## Analysis Overview

The purpose of this analysis is to assess creditworthiness of borrowers by creating and training a model. The financial information in the dataset includes loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory remarks, total debt, and whether their loan is "healthy" or "high-risk". We are trying to predict whether the borrower is high-risk for defaulting on their loan. This is a boolean field, so there are only two choices - 0 (yes, it's healthy), or 1 (no, it's high-risk).

After reading the dataset and splitting it into labels and features, we split the data to train and test it. Next, we fit the model to a logistic regression classifier, and then made predictions with the test data. We created a confusion matrix with the results of the predictions (this shows us how many were actually in each group, and how many we predicted to be in each group). Logistic regression uses one dependent variable and one or more independent variable to predict outcomes.

## Results

* Logistic Regression Model
    * Accuracy: 0.99
    * Precision
        - Healthy: 1.0
        - High-Risk: 0.87
    * Recall
        - Healthy: 1.00
        - High-Risk: 0.89

## Summary

The Logistic Regression model seems to have predicted the healthy loans very well, and it does a good job at predicting the high-risk loans, but it could be better. There were 80 "false positives" - meaning there were 80 high-risk loans that were classified as healthy. This scenario is detrimental to both borrowers and to lending institutions. It is more important to predict the high-risk loans, so perhaps a different model would be better to predict those.





*All code was written by me.*
