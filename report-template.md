# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).


    The purpose of this analysis was to assess the risk associated with loan data based on various financial variables provided in order to determine whether they are healthy or high risk. The analysis focused on variables such as loan size, interest rate, borrower's income, borrower's debt-to-income ratio, number of accounts on file, derogatory marks on the credit report, and total debt of the borrower. The machine learning process involved several stages. Firstly, data preprocessing was performed, which included loading the data, checking its size, and assigning the variables for prediction (X) and the target variable (y). Next, a logistic regression model was trained using the data. The model was then evaluated using metrics such as the balanced accuracy score and confusion matrix. To address the issue of class imbalance, random oversampling was applied. Finally, the results were reported, indicating whether a loan was classified as healthy or high risk


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  
Balanced Accuracy Score (measures how well a model predicts when data is unbalanced)
* 0.9521352751368186
  
Precision(measure of accuracy)
* for class 0 (healthy loans): 1.00 - 100% accuracy
* for class 1 (high-risk loans): 0.86 - 86% of loans predicted were actually high risk
  
  
Recall (sensitivity or true positive)
* for class 0 (healthy loans): 1.00 - 100% accuracy
* for class 1 (high-risk loans): 0.91 - 91% of loans predicted were actually high risk


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  
Balanced Accuracy Score
 * 0.9941749445500477
  
Precision
* for class 0 (healthy loans): 1.00 - 100% accuracy
* for class 1 (high-risk loans): 0.86 - 86% of loans predicted were actually high risk
  
Recall
* for class 0 (healthy loans): 1.00 - 100% accuracy
* for class 1 (high-risk loans): 0.91 - 91%  of loans predicted were actually high risk

 

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
The resampled data model has a higher balanced accuracy score.


* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
The original model is good at predicting a more balanced outcome.

If the goal is only to access high risk than the oversampled model is better.
For the purpose of accessing risk the overfitted model is far superior and the better choice overall.

If you do not recommend any of the models, please justify your reasoning.
Both models performed very well but I would to prefer to test other models as well to make sure the best one is applied. I wouldn't feel comfortable in my analysis unless I tested other options.
