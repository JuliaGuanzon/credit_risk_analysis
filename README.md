<h1 align="center">Credit Risk Analysis Report</h1>

## Overview of the Analysis

Credit risk analysis is important when it comes to lending. In order to make sure a financial or lending institution is not putting their self at risk, they must identify the creditworthiness of their potential borrowers. To identify creditworthy borrowers, information on the borrower's debt to income, loan size, and derogatory marks on credit are taken into account. In order to make sense of the data and find these values useful, an analysis report has been created to assist in predict based off of historical data, which types of borrowers pose a risk.

By using a historical lending activity dataset from a peer-to-peer lending services company, we have been able to train models to evaluate the imbalanced borrower classes. Due to most borrowers having "healthy loans", the data becomes imbalanced as there are not that many borrowers who have "loans at high risk of default". To fix this imbalance, we use logistic regression and resampling to help us arrive to our goal. Our goal is to accurately predict the number of "healthy loans" and "loans at high risk of default". In order to breakdown the data into useful values, we split the "loan_status" from the rest of the data to see if the models could accurately predict the type of loans certain borrowers had.

In order to complete this task, the credit risk model must take the original data and train, test, and split the data. The function *train_test_split* takes 75% of our data and uses it to train the model and 25% of the data to test the model's prediction. Next, we take the training data and model and fit it using logistic regression. Using logistic regression, we predict the model using the testing data. The predicted and actual data are formatted into a binary format and evaluated. The model is evaluated for accuracy, precision, and recall. A classification report is provided to assess the effectiveness our model had on predicting the types of borrowers.

As mentioned above, the imbalance of data makes it difficult to accurately predict, so a resampling of the data is needed to make the model more accurate. Resampled data is used to model and fit using logistic regression. Using logistic regression, we predict the model using the original testing data. The predicted and actual data are formatted into a binary format and evaluated.The new model is evaluated for accuracy, precision, and recall. A classification report is provided to assess the effectiveness our new model had on predicting the types of borrowers.

The models created have been trained to understand what constitutes as "healthy loans" and "loans at high risk of default". These models make accurate predictions, therefore perform perfectly and ready to use.

## Results

<details>
<summary>Machine Learning Model 1</summary>

This model used original data with Logistic Regression. 
 
  * Balance Accuracy Score: 0.95
 
    The model received a high balance accuracy score confirming that this model performs well.
 
  * Precision:
 
    Precision shows how confident the prediction process is for the model. "Healthy Loans" scored a perfect score making the model very confident in predicting. "Loans at High Risk of Default" proves to be less confident than "Healthy Loans", but fairly confident in predicting.
 
     Healthy Loans (0): 1.00
 
     Loans at High Risk of Default (1): 0.85
 
  * Recall:
    
    Recall scores for both "Healthy Loans" and "Loans at High Risk of Default" were very high. As recall measures the actual number of "Healthy Loans" and "Loans at High Risk of Default" the model classifies correctly, meaning that these high scores gives the confidence that the model can classify correctly.
 
     Healthy Loans (0): 0.99
 
     Loans at High Risk of Default (1): 0.91
</details>


<details>
<summary>Machine Learning Model 2</summary>
 
This model used Logistic Regression with resampled training data. 
 
  * Balance Accuracy Score: 0.99
 
    The model received a close to perfect balance accuracy score confirming that this model accurately predicts the data.
 
  * Precision:
 
    Precision shows how confident the prediction process is for the model. "Healthy Loans" scored a perfect score making the model very confident in predicting. "Loans at High Risk of Default" proves to be less confident than model one, but still fairly confident in predicting.
 
     Healthy Loans (0): 1.00
 
     Loans at High Risk of Default (1): 0.84
 
  * Recall:
 
    Recall scores for both "Healthy Loans" and "Loans at High Risk of Default" were nearly perfect. As recall measures the actual number of "Healthy Loans" and "Loans at High Risk of Default" the model classifies correctly, meaning that the model accurately classifies the data with perfection.
 
     Healthy Loans (0): 0.99
 
     Loans at High Risk of Default (1): 0.99
</details>

## Summary

Overall, the machine learning models created in this report were accurate. The initial model scored an average of .96 on its classification report, while the resampling model had an average score of .99 on its classification report. Our main goal was to be able to predict the loans that were at a high risk of defaulting, and both models performed well. The best performing model is model two (with resampling) as it scored much higher on the loans with high risk of defaulting. Model two provides us with an average score of .95 for the high risk of defaulting status, while model one had a score of .91. Although they scored well overall, the focus is on the ability to predict if loans were at a high risk for default, as this data would help us better predict future data trends.

With the models being super accurate, there is a possibility of them becoming problematic in a sense that, in the future, they may not be able to predict when new data is introduced. High accuracy scores are good, but when it is consistently high accross the two models, you must proceed with caution. If a recommendation had to be made, model two would be the best choice to use as it scored the best.

