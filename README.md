# Supervised Learning Model-challenge
Use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

## Overview of the Analysis

In this section, we completed an analysis for various machine learning models that can identify the creditworthiness of borrowers. 
The purpose of the analysis was to identify the most effective model for accurately predicting loan risk.

* Purpose of the analysis: The goal was to predict risk with loan applicant using the historical lending activity from a peer-to-peer lending services company.
* We used finances data related to borrower and loan details to predict whether a loan application will be 'Healthy Loan' - 0 or 'High-Risk Loan' - 1.
* Distribution of target varaible (Loan Status) in Prediction Data - 'Healthy Loan' - 18691 and 'High-Risk Loan' -  693
* Machine learning process stages:
    * Data Pre-processing: Separated the Features and Target in two different sets.
    * Split the cleaned dataset into train and test data.
    * Trained multiple models using different algorithms.
    * Evaluated models based on accuracy, precision, and recall.

Model Training: Trained multiple models using different algorithms.
* Logistic Regression
* KNeighborsClassifier
* Decision Tree
* Random Forest
* Support Vector Machine (SVM)

## Results

    Logistic Regression is 99.246801 percent accurate
    ##################################################
    [[18655   110]
    [   36   583]]
    ---------------------------------------------------------   
                precision    recall  f1-score   support
    ---------------------------------------------------------   
    Healthy Loan       1.00      0.99      1.00     18765
    High-Risk Loan       0.84      0.94      0.89       619

      accuracy                           0.99     19384
     macro avg       0.92      0.97      0.94     19384
    weighted avg       0.99      0.99      0.99     19384

    KNN is 99.329344 percent accurate
    ##################################################
    [[18651   114]
    [   16   603]]
    ---------------------------------------------------------   
                precision    recall  f1-score   support
    ---------------------------------------------------------   
    Healthy Loan       1.00      0.99      1.00     18765
    High-Risk Loan       0.84      0.97      0.90       619

      accuracy                           0.99     19384
     macro avg       0.92      0.98      0.95     19384
    weighted avg       0.99      0.99      0.99     19384

    Linear SVMs is 99.380933 percent accurate
    ##################################################
    [[18649   116]
    [    4   615]]
    ---------------------------------------------------------   
                precision    recall  f1-score   support
    ---------------------------------------------------------   
    Healthy Loan       1.00      0.99      1.00     18765
    High-Risk Loan       0.84      0.99      0.91       619

      accuracy                           0.99     19384
     macro avg       0.92      0.99      0.95     19384
    weighted avg       0.99      0.99      0.99     19384

    Non Linear SVMs is 99.380933 percent accurate
    ##################################################
    [[18651   114]
    [    6   613]]
    ---------------------------------------------------------   
                precision    recall  f1-score   support
    ---------------------------------------------------------   
    Healthy Loan       1.00      0.99      1.00     18765
    High-Risk Loan       0.84      0.99      0.91       619

      accuracy                           0.99     19384
     macro avg       0.92      0.99      0.95     19384
    weighted avg       0.99      0.99      0.99     19384

    Decision Trees is 99.014651 percent accurate
    ##################################################
    [[18668    97]
    [   94   525]]
    ---------------------------------------------------------   
                precision    recall  f1-score   support
    ---------------------------------------------------------   
    Healthy Loan       0.99      0.99      0.99     18765
    High-Risk Loan       0.84      0.85      0.85       619

      accuracy                           0.99     19384
     macro avg       0.92      0.92      0.92     19384
    weighted avg       0.99      0.99      0.99     19384

    Random Forests is 99.164259 percent accurate
    ##################################################
    [[18665   100]
    [   62   557]]
    ---------------------------------------------------------   
                precision    recall  f1-score   support
    ---------------------------------------------------------   
    Healthy Loan       1.00      0.99      1.00     18765
    High-Risk Loan       0.85      0.90      0.87       619

      accuracy                           0.99     19384
     macro avg       0.92      0.95      0.93     19384
    weighted avg       0.99      0.99      0.99     19384



## Summary

The Decision Trees model seems to perform best with an accuracy of 0.99, precision of 0.84, and recall of 0.85. 

The performance does depend on the accuracy of high-risk loans (1) prediction. so, the Decision Trees model's with least True Positive value of 525 is particularly advantageous.




