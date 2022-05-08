# Credit_Risk_Analysis
Module 17

## Overview of the analysis 

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm.  

Compare two new machine learning models, BalancedRandomForestClassifier and EasyEnsembleClassifier that reduce bias, to predict credit risk. Evaluate the performance of these models and make a recommendation on whether they should be used to predict credit risk.

## Results 

The following are balanced accuracy scores, the precision and recall scores of all six machine learning models.

* [RandomOverSampler Method](/images/01_RandomOverSampler.PNG)
```
balanced accuracy score = 0.5057471264367817

            prec    rec
high_risk   1.00    0.01
low_risk    1.00    1.00
avg/total   1.00    1.00
```
* [SMOTE Oversampling](/images/02_SMOTE.PNG)
```
balanced accuracy score = 0.632052971060912

            prec    rec
high_risk   0.01    0.62
low_risk    1.00    0.64
avg/total   0.99    0.64
```
* [ClusterCentroids Undersampling](/images/03_ClusterCentroids.PNG)
```
balanced accuracy score = 0.5293026900499977

            prec    rec
high_risk   0.01    0.61
low_risk    1.00    0.45
avg/total   0.99    0.45
```
* [SMOTEENN Combination (Over and Under) Sampling](/images/04_SMOTEENN.PNG)
```
balanced accuracy score = 0.6375533316412246

            prec    rec
high_risk   0.01    0.70
low_risk    1.00    0.57
avg/total   0.99    0.57
```
* [Balanced Random Forest Classifier](/images/05_BalancedRandomForestClassifier.PNG)
```
balanced accuracy score = 0.7877672625306695

            prec    rec
high_risk   0.04    0.67
low_risk    1.00    0.91
avg/total   0.99    0.91
```
* [Easy Ensemble Classifier](/images/06_EasyEnsembleClassifier.PNG)
```
balanced accuracy score = 0.925427358175101

            prec    rec
high_risk   0.07    0.91
low_risk    1.00    0.94
avg/total   0.99    0.94
```
## Summary 

While two the models produces decent balanced accuracy scores, for this data, I would recommend using the Easy Ensemble Classifier model. The final method produced an accuracy score of 0.9254 which was the highest of all six models run.
