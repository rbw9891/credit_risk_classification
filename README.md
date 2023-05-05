# credit_risk_classification

## Overview of the Analysis

In this Challenge, we trained and evaluated a model based on loan risk to predict healthy vs risky loans. The data given to us for use in the model contained labels of either healthy (0) loans or high-risk loans (1) and seven features that help to determine these labels. The features included loan size, interest rates, borrower income, debt to income ratio, number of accounts of borrower, derogatory marks, and total debt. The balance of the target values (labels) was certainly a bit skewed, having 75,036 healthy loans vs 2,500 high-risk loans. The general stages of the ML process included splitting the data into labels and features, further splitting this data into training and testing, fitting the model with the training data, making predictions using the testing data, and finally evaluating the model by comparing the model prediction labels to the test labels. The model used for this analysis was logistic regression and in the second attempt of the model we used random over samplying in order to deal with the skewedness of the label data.

## Results

Model 1:
    - Accuracy: (~ 0.95)
    - Precision: (0) 1.00, (1) 0.85
    - Recall: (0) 0.99, (1) 0.91

Model 2:
    - Accuracy: (~ 0.99)
    - Precision: (0) 1.00, (1) 0.84
    - Recall: (0) 0.99, (1) 0.99 

## Summary