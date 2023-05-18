# Credit Risk Analysis Report

## Overview of the Analysis
In this analysis we used various machine learning techniques to train and evaluate the performance of Logistic Regression Models in identifying loan risk and the creditworthiness of borrowers. The two models we created were trained using different methods, and their performances were compared to determine the superior model. The predictive variables we used in the model are the labels 0 (healthy loan) and 1 (high-risk loan).

The first step was splitting the dataset into features and labels, and further dividing it into training and testing sets.

The first machine learning model was built by instantiating a logistic regression model and training with the original training sets (X_train, y_train), fitting it to the training sets, and using it to generate predictions.
The second machine learning model was created by resampling the original training data using the RandomOverSampler module, instantiating a logistic regression model and fitting the resampled training sets (X_oversample, y_oversample) to the model, and generating predictions.

The performance of each model was evaluated based on the balance accuracy score, the confusion matrix, the precision score, the recall score, and the f1-score in the classification report.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* ML Model 1:

  ![model 1](https://github.com/robbernstein7/credit-risk-classification/assets/119881903/c2c68e2c-829c-4bc2-b750-cdd14d37162a)

The first model was trained on the original data and it give an accuracy of 94.4% in predicting the 2 labels. The model is very good at predicting the healthy loans, with both precision and recall scores of 1.00. The model did not perform as well in predicting the high-risk loans. The precision score for high-risk loans is 0.87, which shows that only 87% of actual high-risk loans were correctly predicted. The recall score for high-risk loans is 0.89, indicating that the model only identified 89% of all high-risk loans in the dataset.

* ML Model 2:

  ![model 2](https://github.com/robbernstein7/credit-risk-classification/assets/119881903/0267c5c3-6b1b-49fd-bceb-c58ce7371b17)

The second model was trained on the resampled data and has an accuracy of 99.6% in predicting the 2 labels. The model peforms well at predicting the healthy loans, with both precision and recall scores of 1.00. The precision score for high-risk loans remains at 0.87, but the recall score has improved to 1.00, indicating that the model can now predict all high-risk loans in the dataset.
  
## Summary

The analysis appears to shows that Model 2 outperforms Model 1 in predicting high-risk loans and has an overall higher accuracy in predicting both labels. Model 2 achieved a relatively high precision in predicting high-risk loans while also correctly identifying all high-risk loans in the dataset. After analysing the models I would recommend using Model 2 in identifying high-risk loans and overall better accuracy in predicting labels.
