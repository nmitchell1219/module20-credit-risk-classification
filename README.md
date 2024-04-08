# Credit Risk Classification 
Module 20 - Supervised Learning Challenge

## Overview of the Analysis

The purpose of this analysis was to develop machine learning models capable of predicting loan risk for a financial institution. The data comprised various financial metrics, such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The primary objective was to predict the loan status, categorized as 0 (healthy loan) and 1 (high-risk loan).

To approach this challenge, the following stages were undertaken:

🔹Data Preprocessing: The dataset was split into features (X) and the target variable (y), where the target variable was the loan status.<br>
🔹Splitting the Data: The data was divided into training and testing sets to evaluate the model's performance on unseen data.<br>
🔹Model Training and Evaluation: A LogisticRegression model was trained using the training set. The model's performance was then evaluated on the testing set to understand its accuracy, precision, and recall.

## Results

#### Machine Learning Model 1 (Logistic Regression):
🔹Accuracy: The model achieved high accuracy scores, with 99.28% on the training data and 99.26% on the testing data, indicating its strong overall predictive performance.<br>
🔹Precision and Recall:<br>
&nbsp;🔸For healthy loans (0): Nearly perfect with a precision of 1.00 and a recall of 0.99.<br>
&nbsp;🔸For high-risk loans (1): Good, with a precision of 0.84 and a recall of 0.94, demonstrating the model's ability to identify the majority of high-risk loans, albeit with some misclassifications.

## Summary

The Logistic Regression model demonstrates excellent predictive capability, particularly for healthy loans. It also shows a commendable performance in identifying high-risk loans, making it a valuable tool for financial institutions aiming to minimize risk.

The choice between emphasizing precision or recall in this context depends on the financial institution's risk appetite. If the priority is to minimize false negatives (i.e., failing to identify high-risk loans), focusing on recall for high-risk loans would be crucial. Conversely, if reducing false positives (i.e., incorrectly labeling loans as high-risk) is more important, precision becomes the key metric.

Given the model's high performance across both metrics for healthy loans and its respectable identification of high-risk loans, it appears well-suited for the task. However, for applications where identifying every potential high-risk loan is critical, further tuning or exploring more complex models might be necessary to improve recall for the 1 class without significantly compromising precision.
