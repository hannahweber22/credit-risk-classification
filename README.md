# credit-risk-classification

## Overview of the Analysis

# In this module, I used a variety of techniques to train and evaluate a model based on loan risk. The dataset is of historical lending activity from a peer-to-peer lending services company. The model identifies the creditworthiness of borrowers. The variables I predicted during the analysis were the y.value counts to see the balance of labels, and the accuracy score, confusion matrix and classification report to see how accurate the model is performaning. I went through splitting the data into training and testing data, fitting the training data to a logistic regrssion model, predicting the testing data, refitting the training data to a randomoversampler model, and repredicting the testing data to the logistic model.The methods used were the LogisticRegression and RandomOverSampler. 


## Results

# Machine Learning Model 1:
# The logistic regression model predicts the healthy loan ('0') with a 
 - 100% precision
 - 100% recall
 - 100% f1-score
# The high-risk loan is predicted w/ a 
 - 87% precision
 - 89% recall 
 - 88% f1-score
# The healthy loan uses a lot more support data points of 18759 than the high-risk loan of 625. Both the healthy and high-risk loans are predicted very well. 

#  Machine Learning Model 2:
# The regression model, fit w/ oversampled data, predicts the data better. The healthy loan ('0') still has a 
 - 100% precision
 - 100% recall
 - 100% f1-score
# The high-risk loan is now 
 - 87% precision
 - 100% recall 
 - 93% f1-score
# The healthy loan uses a lot more support data points of 18759 than the high-risk loan of 625. Both the healthy and high-risk loans are predicted very well. 

## Summary

# The model where the training data is fit w/ the RandomOverSampler model and predicted w/ the LogisticRegression models seems to perform slightly better based on the classification report. I believe it would be more important to predict '1's to determine if a loan is high risk. It would be important for the model to be able to determine high risk loans and point those out. A mistake of missing a high risk loan is probably more costly than missing a healthy loan. 