# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

The main goal of this analysis was to use and evaluate machine learning models based on loan risk. The finanical information we focused on was "loan_status" and the categories for this were '0' (healthy loan) and '1' (high-risk-loan). For the machine learning aspect I used the following steps;
1) Read all of the data from the CSV file
2) Create labels from the "loan_status" column and create a seperate DataFrame with that column removed
3) Split the data into Training and Testing Sets using "train_test_split" from sklearn
4) Create a Logistic Regression Model with the Training Data
5) Save the predictions on the testing data labels using the testing feature data
6) Evaluate the models performance by generating a confusion matrix & classification report
The main method we used was 'LogisticRegression' to create our model with the original data.


## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

The model had 100% precision for all loans in the '0' category (healthy loans) and 85% precision for loans in the '1' category (high-risk-loans). The model has a weighted average of 99% due to there being 5X as many healthy loans compared to high risk loans.


              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384


## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

I think this model is adequate. I would want to compare it against another to see if we can find something more precise. If I was working for the company looking at these loans I'd be more concerned with the high-risk-loans and the model we used only had 85% precision on this. These are the loans mor elikely to default and cost the company money so I'd feel much better about or model if our results were flipped.


If you do not recommend any of the models, please justify your reasoning.
