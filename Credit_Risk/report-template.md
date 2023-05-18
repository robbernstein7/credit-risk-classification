# Module 12 Report Template

## Overview of the Analysis
In this analysis we used various machine learning techniques to train and evaluate the performance of Logistic Regression Models in identifying loan risk and the creditworthiness of borrowers. The two models we created were trained using different methods, and their performances were compared to determine the superior model. The predictive variables we used in the model are the labels 0 (healthy loan) and 1 (high-risk loan).

The first step was splitting the dataset into features and labels, and further dividing it into training and testing sets.

The first machine learning model was built by instantiating a logistic regression model and training with the original training sets (X_train, y_train), fitting it to the training sets, and using it to generate predictions.
The second machine learning model was created by resampling the original training data using the RandomOverSampler module, instantiating a logistic regression model and fitting the resampled training sets (X_oversample, y_oversample) to the model, and generating predictions.

The performance of each model was evaluated based on the balance accuracy score, the confusion matrix, the precision score, the recall score, and the f1-score in the classification report.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* ML Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.



* ML Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
