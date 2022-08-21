# Credit_Risk_Analysis

## Overview
The purpose of this analysis is to apply supervised machine learning techniques to assess credit card risk.  The number of good credit card loans vastly outnumbers bad loans creating an inherently imbalanced classification problem where different techniques will be used to train and evaluate models with unbalanced classes.  The data will first be oversampled using RandomOverSampler and SMOTE algorithms and then the data will be undersampled using ClusterCentroids algorithm. A combined approach will then be taken, of over and under sampling the data with the SMOTEEN algorithm.  Finally to reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier will be used to predict credit risk.    

## Results
#### RandomOverSampler:
![RandomOverSampling_bascore](https://user-images.githubusercontent.com/103215123/185773360-c2db74eb-0324-437e-bb32-b374c6c6a5f3.png)
![RandomOverSampling](https://user-images.githubusercontent.com/103215123/185773370-e524767a-ab72-43de-bdc4-dc157136ef10.png)
- Balanced Accuracy Score is 64.6%
- Precision for high risk is 1%, Precision for low risk is nearly 100% 
- Sensitivity for high risk is 71% and Sensitivity for low risk loans is 58%

#### SMOTE Oversampling:
![SMOTE_bascore](https://user-images.githubusercontent.com/103215123/185773377-660b5e03-5050-4756-ac5c-55d3de874152.png)
![SMOTE_cr](https://user-images.githubusercontent.com/103215123/185773381-430789b7-544a-49d6-9272-89abf6e470ce.png)
- Balanced Accuracy Score is 65.8%
- Precision for high risk is 1%, Precision for low risk is nearly 100%
- Sensitivity for high risk is 63% and Sensitivity for low risk is 68%
- 

#### ClusterCentroids Undersampling:
![ClusterCentroids_bascore](https://user-images.githubusercontent.com/103215123/185773008-d7db627b-336e-432e-ac6a-bc300472880c.png)
![ClusterCentroids_cr](https://user-images.githubusercontent.com/103215123/185773019-699ba16a-89ec-4c62-9172-6496ef1c1e6b.png)
- Balanced Accuracy Score is 54.4%
- Precision for High Risk is 1%, Precision for Low Risk is 100%
- Sensitivity for High Risk is 68% and Sensitivity for Low Risk is 63%


#### SMOTEEN Combination Over/Undersampling:
![SMOTEEN_bascore](https://user-images.githubusercontent.com/103215123/185773031-cd339c09-866f-455a-ab8b-62c55ae3499c.png)
![SMOTEEN_cr](https://user-images.githubusercontent.com/103215123/185773037-96d239f1-9900-463f-85f0-1cc19e1bcb5d.png)
- Balanced Accuracy Score is 64.8%
- Precision for High Risk is 1% and Precision for Low Risk is nearly 100%
- Sensitivity for High Risk is 72%, Sensitivity for Low Risk is 57%

#### BalancedRandomForestClassifier:
![BalancedRandomForest_bascore](https://user-images.githubusercontent.com/103215123/185773149-6e6f5761-c233-480b-9cff-fad8786ee4da.png)
![BalancedRandomForest_cr](https://user-images.githubusercontent.com/103215123/185773153-c121f497-c79a-4766-bbf4-c2ea41a883ce.png)
- Balanced Accuracy Score is 78.8% 
- Precision for High Risk is 3%
- Sensitivity for High Risk is 70% and for Low Risk is 87%


#### EasyEnsembleClassifier:
![EasyEnsemble_bascore](https://user-images.githubusercontent.com/103215123/185773231-3e43b824-f92c-4ce9-ba54-4e101226462e.png)
![EasyEnsemble_cr](https://user-images.githubusercontent.com/103215123/185773235-303978c9-078e-4fb3-9818-4edfcdb82466.png)
- Balanced Accuracy Score is 92.6%
- Precision for High Risk is 8% 
- Sensitivity for High Risk is 90% and Low Risk is 95% 


## Summary
The accuracy or precision of the oversampling models, undersampling models, and combination models is significantly lower than the Balanced Random Forest and Easy Ensemble classifiers.  With this weaker performance in predicting higher risk loans, I would reccommend that LendingClub, if they were to use any of these models for predicting high risk credit card loans, that they use the Balanced Random Forest classifier or the Easy Ensemble Classifier models.  
