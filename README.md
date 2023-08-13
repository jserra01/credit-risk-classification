# Module 20 Supervised Learning Report

## Overview of the Analysis

We evaluted historical data from a peer-to-peer lending services company to build a model to identify credit worthiness of customers and whether their loan has a high risk of defaulting.  Financial information available for this analysis is:

Features:
* Loan Size
* Interest Rate
* Borrower Income
* Debt to Income Ratio
* Number of Accounts
* Number of Derrogatory Marks
* Total Debt

Target:
* Loan Status: High Risk (1) vs. Healthy (0)

## Approach

Our intent with this analysis is to predict loan status based on available historical data.  This data for loan status consisted of 77,536 loans with 75,036 (97%) healthy loans and 2,500 (3%) high-risk loans.  To accomplish this anlayis, we used Logistic Regression to build our models.  After splitting the data into training and testing samples, we built our first model with the original data set.  Given the large discrepancy in data towards the health loans, we built a second model and oversampled the high-risk loans using 

## Results

* Machine Learning Model 1: Original Data
  * Model 1 Accuracy: 99%
  * Healthy Loan Precision: 100%
  * Healthy Loan Recall: 99%
  * High-Risk Loan Precision: 85%
  * High-Risk Loan Recall: 91%

* Machine Learning Model 2: Resampled Data - oversampling High-Risk loans
  * Model 1 Accuracy: 99%
  * Healthy Loan Precision: 100%
  * Healthy Loan Recall: 99%
  * High-Risk Loan Precision: 84%
  * High-Risk Loan Recall: 99%

## Summary

Similar results achievied for both models with an accuracy of 99% and relatively low precision on High-Risk loans (85% for Model 1 vs 84% for Model 2).  Given that it is more important to predict High-Risk loans and the higher reall in Model 2 and relatively similar precision between both models, my recommendation is to use Model 2.  Although, I would recommend exploring additional features/data elements and possibly increasing the sample size to build a better model and continue to strive for better prediction of High-Risk loans.

## Sources
(https://machinelearningmastery.com/random-oversampling-and-undersampling-for-imbalanced-classification/)[Machine Learning Mastery]: oversampling example
