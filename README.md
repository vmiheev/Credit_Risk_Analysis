# Credit_Risk_Analysis

## Overview

Using machine learning to predict the credit risk of customers for a peer-to-peer lending services company.

## Results

### Logistic Regression Model

The dataset has a class imbalance favouring low-risk clients (high-risk clients: 347; low-risk clients: 68470). To account for this, the Logistic Regression Model has been used on a four different sampling methods of the dataset:

* Naive Random Oversampling
Balanced accuracy score: 0.648072305476572
Precision (high-risk clients): 0.01
Recall (high-risk clients): 0.69

![Naive Random Oversampling](/Results/Naive_Random_Oversampling.png)

* SMOTE Oversampling
Balanced accuracy score: 0.6625695222702812
Precision (high-risk clients): 0.01
Recall (high-risk clients): 0.63

![SMOTE Oversampling](/Results/SMOTE_Oversampling.png)

* Cluster Centroids Undersampling
Balanced accuracy score: 0.5473255054691625
Precision (high-risk clients): 0.01
Recall (high-risk clients): 0.68

![Cluster Centroids](/Results/Cluster_Centroids.png)

* SMOTEENN
Balanced accuracy score: 0.636963792847947
Precision (high-risk clients): 0.01
Recall (high-risk clients): 0.69

![SMOTEENN](/Results/SMOTEENN.png)

### Logistic Regression Model



## Summary

* 