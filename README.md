# credit_risk_classification

## Overview of the Analysis

In this Challenge, we trained and evaluated a model based on loan risk to predict healthy vs risky loans. The data given to us for use in the model contained labels of either healthy (0) loans or high-risk loans (1) and seven features that help to determine these labels. The features included loan size, interest rates, borrower income, debt to income ratio, number of accounts of borrower, derogatory marks, and total debt. The balance of the target values (labels) was certainly a bit skewed, having 75,036 healthy loans vs 2,500 high-risk loans. The general stages of the ML process included splitting the data into labels and features, further splitting this data into training and testing, fitting the model with the training data, making predictions using the testing data, and finally evaluating the model by comparing the model prediction labels to the test labels. The model used for this analysis was logistic regression and in the second attempt of the model we used random over samplying in order to deal with the skewedness of the label data.

## Results

* Model 1:
    - Accuracy: (~ 0.95)
        > The balanced accuracy score of the model was approximately 0.95 (1.00 being the highest)
          and was used instead of a regular accuracy score in order to handle the imbalanced data. It is the avg of recalls from each class (label).
    - Precision: (0) 1.00, (1) 0.85
        > The precision scores were 1.00 for healthy loans and 0.85 for high-risk loans. This means that out of all the loans that the model predicted would be healthy, 100% actually were. And out of all the loans the model predicted would be high-risk, 85% actually were.
    - Recall: (0) 0.99, (1) 0.91
        > The recall scores were 0.99 for healthy loans and 0.91 for high-risk loans. This means that out of all the loans that were healthy, the model predicted this outcome 100% of the time. And out of all the loans that were high-risk, the model predicted this outcome 91% of the time.

* Model 2:
    - Accuracy: (~ 0.99)
         > The balanced accuracy score of the model was approximately 0.99 (1.00 being the highest)
          and was used instead of a regular accuracy score in order to handle the imbalanced data. It is the avg of recalls from each class (label).
    - Precision: (0) 1.00, (1) 0.84
        > The precision scores were 1.00 for healthy loans and 0.84 for high-risk loans. This means that out of all the loans that the model predicted would be healthy, 100% actually were. And out of all the loans the model predicted would be high-risk, 84% actually were.
    - Recall: (0) 0.99, (1) 0.99
        > The recall scores were 0.99 for healthy loans and 0.99 for high-risk loans. This means that out of all the loans that were healthy or high risk, the model predicted this outcome 99% of the time.

## Summary

In the world of lending, one wants to keep the amount of risky loans low. Risky loans tend to not be paid in full as much as healthy ones do and if they don't get paid then lending businesses don't get their money back and certainly don't turn a profit. So, for this scenario keeping the amount of false negatives on high-risk loans is our most important goal. False negatives on high risk loans means that the model would predict the loan to not be high-risk when in actuality the loan was high-risk. In order to evaluate a model for false negatives, it is best to use recall. The higher the recall the lower the amount of false negatives. From the results above, one can easily see that the recall of high-risk (1) loans is higher in the second model compared to the first. Therefore, I would recomend the use of the second model, especially considering the recall is 0.99, near perfect.  