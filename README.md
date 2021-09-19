<h1 align="center">Credit Risk Analysis Report</h1>

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

<details>
<summary>Machine Learning Model 1:</summary>

This model used original data with Logistic Regression. In summary, this model scored very well and had nearly a perfect score for predicting "Healthy Loans". The "Loans at High Risk of Default" scored high in recall, which measures the actual number of "Loans at High Risk of Default" the model classified correctly, and scored moderately high in precision, meaning the model was fairly confident in the prediction process. The model received a high balance accuracy score confirming that this model performs well.
 
  * Balance Accuracy Score: 0.95
 
  * Precision:
 
     Healthy Loans (0): 1.00
 
     Loans at High Risk of Default (1): 0.85
 
  * Recall:
 
     Healthy Loans (0): 0.99
 
     Loans at High Risk of Default (1): 0.91
</details>


<details>
<summary>Machine Learning Model 2:</summary>
 
 
 
  * Balance Accuracy Score: 0.95
 
  * Precision:
 
     Healthy Loans (0): 1.00
 
     Loans at High Risk of Default (1): 0.85
 
  * Recall:
 
     Healthy Loans (0): 0.99
 
     Loans at High Risk of Default (1): 0.91
</details>

## Summary

Overall, the machine learning models created in this report were accurate. The initial model scored an average of .96 on its classification report, while the resampling model had an average score of .99 on its classification report. Our main goal was to be able to predict the loans that were at a high risk of defaulting, and both models performed well. The best performing model is model two (with resampling) as it scored much higher on the loans with high risk of defaulting. Model two provides us with an average score of .95 for the high risk of defaulting status, while model one had a score of .91. Although they scored well overall, the focus is on the ability to predict if loans were at a high risk for default, as this data would help us better predict future data trends.

With the models being super accurate, there is a possibility of them becoming problematic in a sense that, in the future, they may not be able to predict when new data is introduced. High accuracy scores are good, but when it is consistently high accross the two models, you must proceed with caution. If a recommendation had to be made, model two would be the best choice to use as it scored the best.

