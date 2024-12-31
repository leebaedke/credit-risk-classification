  # credit-risk-classification

## Overview of the Analysis

* This analysis trains a machine learning model to predict and differentiate between healthy loans and high risk loans.
* We are using 'loan status' in our training of the model. Other data factors that are present in the data set are: loan size,
 	interest rate,	borrower income, debt to income,	num of accounts, derogatory marks,	total debt.
* There are two variables within 'loan status'. '0' is considered a healthy loan, while '1' is considered having a high risk of defaulting.
  There are 18765 occurrences of '0' and 619 occurrences of '1' in this data set.
* The training of this model started with reading in the dataset and separating out the 'loan status' column from the rest of the dataset.
  Then the data was split into training and testing datasets, then fit to a logistic regression model using the training data. A prediction was then
  made on the fitted model. Lastly a confusion matrix was generated and a classification report was printed.
* Logistic Regression was the primary method used in this analysis.
   
## Results

* Machine Learning Model:
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.84      0.94      0.89       619

    accuracy                           0.99     19384
   macro avg       0.92      0.97      0.94     19384
weighted avg       0.99      0.99      0.99     19384

* This model had 100% Precision predicting healthy loans and 84% predicting high risk loans.
* The Recall of healthy loans was 99%, meaning that in the case of 'true positives', 99% were identified correctly.
  The Recall of high risk loans was 94%, meaning that in the case of 'true positives', 94% were identified correctly.
* The Accuracy of the entire model, all loans, was 99%.

## Summary

* I recommend using this model as a predictor for issuing healthy loans. The near 100% accuracy of predicting a good loan is great for the business.
  However, the rate for predicting high risk of default isn't great, but it is still pretty good. At 84%, it will predict most of the high risk loans, but could still miss 16%.
    
