# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis: 
- The purpose of this analysis is to try and identify a correlation between healthy & high risk loans 

* Explain what financial information the data was on, and what you needed to predict:
- The data was ultimately comparing a clients loan request to their financial data to ultimately try predict their eligibility of a loan.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`):
- The model is looking at the clients financial information such as income and debt to determine if their loan request is a healthy one or not.

* Describe the stages of the machine learning process you went through as part of this analysis.
- To initialise the analysis, an X & y varaiable were implemented. The y representing the loan_status, and the X representing everything but the loan_status.

- Furthermore, the X and y data would be split into training and testing sets. As the model makes predictions, the train and test variables would be used to assess the predictions of the model, and train it on the X data to gradually increase the models accuracy more and more.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
- The LogisticRegression includes a classifier which is fitted to the training variables. Ultimately this allows the model to look over the data x amount of times, to hopefully distinguish a correlation between healthy and high risk loans.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  The model for healthy loans scored 1.0 across all fields, indicating the model was able to correctly identify all healthy loans correctly.



* Machine Learning Model 2:
Still highly accurate, but slightly less successful, the model for high risk loans has an f1-score of .88 (88%). Looking deeper, there is a .02 difference in favour of the recall score .89, meaning there were slightly more occurances where a healthy loan was incorrectly identified as a high-risk loan.

## Summary

Overall, this model was highly accurate. Where the model is inaccurate, it is not good from the banks point of view because if high-risk loans are being identified as healthy, ineligable borrowers are recieving money they may not get returned. 

However these incorrect identifications are likely borderline to eligable loans,

As there are multiple fields and factors incorporated in the dataset, it is necessary to have a well trained model to determine if a loan_status is healthy or high-risk.

However if a direct correlation were to be discovered between healthy and high-risk loan status, that opens up an avenue to having fixed methods of sorting that don't require machine learning.
