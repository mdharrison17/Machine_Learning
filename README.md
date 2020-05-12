# Machine_Learning
Module 17

## Project Overview
Using a dataset from LendingClub and building and evaluate 4 different machine learning algorithms and analyze how they do at predicting credit risk.

## Analysis

### Naïve Random Oversampling
The balance accuracy score is 63.9%.  The precision score for low-risk is 1 and the precision score for high risk is .01.  The Recall score for low risk is .57 and the recall score for high risk is .73.

### SMOTE Oversampling
The balance accuracy score is 65%, the highest of all of the learning models.  The precision score for low-risk is 1 and high risk is .01.  The recall score for low-risk is .68 and high risk is .59.

### Cluster Centroids

The balance accuracy score is 63.9%, same as random oversampling.  The precision score for low-risk is 1 and high risk is .01.  The recall score for low-risk is .39 and high-risk is .69. 

### SMOTEEN
The model with the worst accuracy score at 54.3%.  The precision score for low-risk is 1 and high risk is .01.  The recall score for low-risk is .57 and high-risk is .74.

### Recommendation
I would not recommend any of these methods to predict high and low risk loan applicants.  The highest accuracy score is 65%, but the precision and recall score are not good enough to justify.  All of the machine learning methods have the same precision scores for high and low credit, which are opposite.  Low-risk is 100% and high risk is only .01%.  The problem with all of the models is the high false positive predicted transactions.  The models all predicted a applicants to be high-risk when they were really low-risk.  This puts a lot of actual good applicants in the bad applicants category.  The recall scores are pretty high for most test. Cluster Centroids did the worst and SMOTEEN had the best sensitivity scores.  None of these models have a good balance between precision and sensitivity.  I think with the high accuracy scores, the models have overfitted the datasets.  I would suggest using a model such as random forest algos to help against the overfitting these models clearly have.
