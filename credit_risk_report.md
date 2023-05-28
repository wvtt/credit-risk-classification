# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

The purpose of the analysis is to utilize machine learning to train and evaluate the performance of LR (Logistic Regression) models to identify credit risks from borrowers. Predictive variables in the model are the labels 0 (healthy loan) and 1 (high-risk loan).

The dataset was split into features and labels, which were then divided into training and testing sets used to construct the model.
* Model 1 was built by instantiating a logistic regression model and training with the original training sets (X_train, y_train), fitting it to the training sets, and using it to generate predictions. 
* Model 2 was created by resampling the original training data using the RandomOverSampler module, instantiating a logistic regression model and fitting the resampled training sets (X_resample, y_resample) to the model, and generating predictions.

The performance of each model was evaluated based on the balance accuracy score, the confusion matrix, as well as the precision score, recall score, and f1-score in the classification report.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  
  The model predicted two labels with an accuracy of 94.4% accuracy. The model is accurate at predicting the healthy loans, with an f1-score of 1.00, while the model's accuracy when predicting the high-risk loans can be improved, with an accuracy of 87% on all actual high-risk loans and 89% of all high-risk loans in the dataset. The precision score for high-risk loans is 0.87, indicating that only 87% of actual high-risk loans were correctly predicted. The recall score for high-risk loans is 0.89, indicating that the model only identified 89% of all high-risk loans in the dataset.

* Machine Learning Model 2:
  
  The model was trained on resampled data and has an accuracy of 99.6% in predicting the 2 labels. The model peforms well at predicting the healthy loans, with both precision and recall scores of 1.00. The precision score for high-risk loans remains the same at 0.87, while the recall score has improved to 1.00 meaning the model can predict all high-risk loans in the dataset.

## Summary
    
In conclusion, Model 2 outperforms Model 1 in predicting high-risk loans and has an overall higher accuracy in predicting both labels. Model 2 achieved a relatively high precision in predicting high-risk loans while correctly identifying all high-risk loans in the dataset. Overall, Model 2 is better suited for identifying high-risk loans and overall better accuracy in predicting labels.
