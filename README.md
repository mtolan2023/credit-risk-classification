### Credit Risk Classification

Module 20 Challenge

## Overview of the Analysis

This report examines the usefulness of a supervised-learning model for predicting the credit-worthiness of borrowers for peer-to-peer lending. The dataset used contained a variety of borrower data including loan size, interest rate, borrower income, DTI, number of accounts, derogatory credit marks, total debt, and loan status (healthy or at-risk). The model attempt to predict the "loan status" based on the other factors. 

The taining dataset includes 77,536 loans, of which 75,036 (93%) were healthy and 2,500 (3%) were unhealthy. We attempt to tackle this imbalance using our second Machine Learning Model(random oversampling). We are using SciKit Learn via Python for our analysis. We employed a Logistic Regression Model after splitting our "loan status" data off from our remaining features (borrower info, loan amount etc.). We then split our data into training and testing sets (for employment and scoring of the model) and evaluated the score of the training data against the testing data. We chose to use a balanced accuracy score to test the accuracy of the model since the data was imbalanced and then used a second model based on random oversampling to balance the 2 loan statuses. We measured the accuracy, recall and precision of both models, the results of which are below.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1 (original data):
  
  * Balanced Accuracy: 95.2%
  * Precision: Healthy Loans: 100%, Unhealthy Loans: 85%
  * Recall: Healthy Loans: 99%, Unhealthy Loans: 91%
    
* Machine Learning Model 2 (random oversampling):
  * Balanced Accuracy: 99.36%
  * Precision: Healthy Loans: 100%, Unhealthy Loans: 99%
  * Recall: Healthy Loans: 84%, Unhealthy Loans: 99%

## Summary

Overall, our random oversampled model performs very well with a balanced accuracy score of 99%. We believe that it would be valuable to implement this model to evaluate credit-worthiness of potential borrowers. While both models did very well to identify healthly loans, the improved recall of the oversampled model achieved 99% success in identifying at-risk borrowers. The precision was 84%, meaning that our model has more of a chance of over-predicting risk to underpredicting risk, which would likely be deemed acceptable/necessary for business. 

