## Credit Risk Classification

Module 20 Challenge

## Overview of the Analysis

This report examines the usefulness of a supervised-learning model for predicting the credit-worthiness of borrowers for peer-to-peer lending. The dataset used contained a variety of borrower data including loan size, interest rate, borrower income, DTI ratio, number of accounts, derogatory marks, total debt and loan status (healthy or at-risk). The model attempt to predict the "loan status" based on the other factors. 

The taining dataset includes 77,536 loans, of which 75,036 (93%) were healthy and 2,500 (3%) were unhealthy. We attempt to tackle this imbalanced using our second Machine Learning Model. We are using SciKit Learn via Python for our analysis. We employed a Logistic Regression Model after splitting our loan_status data off from our remaining features (borrower info, loan amount etc.). We then split our data into training and testing sets (for employment and scoring of the model) and evaluated the score of the training data against the testing data. We chose to use a balanced accuracy score to test the accuracy of the model since the data was imbalanced and then used a second model based on random oversampling to balance the 2 loan statuses.

* Explain the purpose of the analysis. DONE
* Explain what financial information the data was on, and what you needed to predict. DONE
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`). DONE
* Describe the stages of the machine learning process you went through as part of this analysis. DONE
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method). DONE

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

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
