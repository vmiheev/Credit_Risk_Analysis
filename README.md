# Credit_Risk_Analysis

## Overview

Using machine learning to predict the credit risk of customers for a peer-to-peer lending services company.

## Results

### Logistic Regression Model

The dataset has a class imbalance favouring low-risk clients (high-risk clients: 347; low-risk clients: 68470). To account for this, the Logistic Regression Model has been used on a four different sampling methods of the dataset:

* Naive Random Oversampling
* Balanced accuracy score: 0.648072305476572
* Precision (high-risk clients): 0.01
* Recall (high-risk clients): 0.69

![Naive Random Oversampling](/Results/Naive_Random_Oversampling.png)

* SMOTE Oversampling
* Balanced accuracy score: 0.6625695222702812
* Precision (high-risk clients): 0.01
* Recall (high-risk clients): 0.63

![SMOTE Oversampling](/Results/SMOTE_Oversampling.png)

* Cluster Centroids Undersampling
* Balanced accuracy score: 0.5473255054691625
* Precision (high-risk clients): 0.01
* Recall (high-risk clients): 0.68

![Cluster Centroids](/Results/Cluster_Centroids.png)

* Balanced accuracy score: 0.636963792847947
* Precision (high-risk clients): 0.01
* Recall (high-risk clients): 0.69

![SMOTEENN](/Results/SMOTEENN.png)

### Balanced Random Forest Classifier

* Balanced accuracy score: 0.7885466545953005
* Precision (high-risk clients): 0.03
* Recall (high-risk clients): 0.70

![Balanced Random Forest Classifier](/Results/Balanced_Random_Forest.png)

### Easy Ensemble AdaBoost Classifier

* Balanced accuracy score: 0.9316600714093861
* Precision (high-risk clients): 0.09
* Recall (high-risk clients): 0.92

![Easy Ensemble AdaBoost](/Results/Easy_Ensemble_AdaBoost.png)

## Summary

* The Logistic Regression Model had lackluster performance on all 4 resamples; the accuracy score did not go over 66% and the Recall did not go over 69%
* The Balanced Random Forest Classifier had good results; it had a fairly high accuracy score of 79%, a Recall of 70% and a slightly improved Precision of 3%
* The Easy Ensemble AdaBoost Classifier had great results; it had a very high accuracy score of 93%, a Recall of 92% and a slightly improved Precision of 9%
* The Easy Ensemble AdaBoost Classifier is the recommended model to use for this dataset; its accuracy score shows that it predicted 93% of the data points in the test data, and its Recall score - the most important evaluation in this dataset - shows that it found 92% of all high risk loans; the Precision, showing that only 9% of high risk predictions by the model will actually be high risk, is not as important in this case as decision makers should stay on the side of safety.