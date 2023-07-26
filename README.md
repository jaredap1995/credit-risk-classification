# Module 20 Report

## Overview of the Analysis

The purpose of the analysis was to apply machine learning models to predict financial data, specifically to identify high-risk loans. This would allow lenders to mitigate their risk by being informed about the potential default likelihood of a loan applicant.

The dataset contained information about the financial history and loan repayment capability of various customers. The machine learning models were trained to predict whether a loan is of high risk (represented by 1) or low risk (represented by 0). 

The number of low-risk loans (represented by 0) was significantly larger (18765 instances) than high-risk loans (represented by 1, with 619 instances), indicating an imbalanced dataset.

The machine learning process began with data preprocessing, including cleaning the data, encoding categorical data, and splitting the data into training and test sets. Subsequently, machine learning models were trained using the training data and the performance of these models was evaluated on the test data.

A logistic regression model was used on the normal unbalanced data and resampled data.

## Results

* Machine Learning Model 1 (Logistic Regression):
  * The model showed high overall accuracy with 99% correct predictions. It showed excellent performance in predicting low-risk loans (0) with precision and recall scores of 1.00 and 0.99 respectively. For high-risk loans (1), the model exhibited a precision of 0.85 and a recall of 0.91. 

* Machine Learning Model 2 (Resampling Method):
  * The second model also showed a similar overall accuracy of 99%. For low-risk loans (0), the precision and recall scores were 1.00 and 0.99, closely matching the first model. However, for high-risk loans (1), the model showed a slightly lower precision of 0.84 but a higher recall of 0.99 when compared to the first model.

## Summary

Both models performed extremely well with almost equivalent accuracy scores of 99%. However, the task is to identify high-risk loans (1), which makes the recall score for predicting high-risk loans a significant metric. Recall, also known as sensitivity or true positive rate, is crucial here as it measures the models' ability to find all the high-risk loans.

Although the first model has a higher precision for high-risk loans, the second model (Resampling Method) outperforms the first with a recall of 0.99 compared to 0.91 from the Logistic Regression model. This indicates that the second model is superior in identifying high-risk loans, which is our main objective.

Therefore, based on this analysis, I would recommend using the second model (Resampling Method) as it is more effective for our goal of predicting high-risk loans, despite its slightly lower precision. This choice prioritizes the ability to correctly identify as many high-risk loans as possible over the risk of incorrectly labeling some low-risk loans as high risk.
