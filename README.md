# Credit_Risk_Analysis

## Overview
The purpose of this analysis is to apply supervised machine learning techniques to assess credit card risk.  The number of good credit card loans vastly outnumbers bad loans creating an inherently imbalanced classification problem where different techniques will be used to train and evaluate models with unbalanced classes.  The data will first be oversampled using RandomOverSampler and SMOTE algorithms and then the data will be undersampled using ClusterCentroids algorithm. A combined approach will then be taken, of over and under sampling the data with the SMOTEEN algorithm.  Finally to reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier will be used to predict credit risk.    

## Results
#### RandomOverSampler:
![RandomOverSampling_bascore](https://user-images.githubusercontent.com/103215123/185772124-9ae8d764-d9e7-4476-a6bd-5043bfa80ed2.png)
![RandomOverSampling](https://user-images.githubusercontent.com/103215123/185772128-a879d856-f5e4-4e07-ae14-d97a2686d250.png)
- Balanced Accuracy Score is 64.6%
- Precision for high risk is 1%, Precision for low risk is nearly 100% 
- Sensitivity for high risk is 71% and Sensitivity for low risk loans is 58%

#### SMOTE Oversampling:
![SMOTE_bascore](https://user-images.githubusercontent.com/103215123/185772405-5e7c0c55-79f5-4154-91d6-5c21e33bf666.png)
![SMOTE_cr](https://user-images.githubusercontent.com/103215123/185772408-374422e4-7fe9-4f5c-825b-314173b52d8e.png)
- Balanced Accuracy Score is 65.8%
- Precision for high risk is 1%, Precision for low risk is nearly 100%
- Sensitivity for high risk is 63% and Sensitivity for low risk is 68%

#### ClusterCentroids Undersampling:
![ClusterCentroids_bascore](https://user-images.githubusercontent.com/103215123/185773008-d7db627b-336e-432e-ac6a-bc300472880c.png)
![ClusterCentroids_cr](https://user-images.githubusercontent.com/103215123/185773019-699ba16a-89ec-4c62-9172-6496ef1c1e6b.png)


#### SMOTEEN Combination Over/Undersampling:
![SMOTEEN_bascore](https://user-images.githubusercontent.com/103215123/185773031-cd339c09-866f-455a-ab8b-62c55ae3499c.png)
![SMOTEEN_cr](https://user-images.githubusercontent.com/103215123/185773037-96d239f1-9900-463f-85f0-1cc19e1bcb5d.png)

#### BalancedRandomForestClassifier:
![BalancedRandomForest_bascore](https://user-images.githubusercontent.com/103215123/185773149-6e6f5761-c233-480b-9cff-fad8786ee4da.png)
![BalancedRandomForest_cr](https://user-images.githubusercontent.com/103215123/185773153-c121f497-c79a-4766-bbf4-c2ea41a883ce.png)


#### EasyEnsembleClassifier:
![EasyEnsemble_bascore](https://user-images.githubusercontent.com/103215123/185773231-3e43b824-f92c-4ce9-ba54-4e101226462e.png)
![EasyEnsemble_cr](https://user-images.githubusercontent.com/103215123/185773235-303978c9-078e-4fb3-9818-4edfcdb82466.png)


## Summary
