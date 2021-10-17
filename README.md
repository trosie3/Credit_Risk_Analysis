# Credit_Risk_Analysis

## Overview of the analysis: 
The purpose of this analysis is find the best fit machine learning model to predit credit risk for those appying for loans. For this model the ideal outcome is a method that predicts high-risk well. Methods analyzed for best model: Over-sampling RandomOverSampler and SMOTE, Under-sampling ClusterCentroids, Combined-sampling methord SMOTEEENN, and ensemble methods of BalancedRandomForestClassifier and EasyEnsembleClassifier.

## Results: 
Model evualtion numbers by method:
- Random

![image](https://github.com/trosie3/Credit_Risk_Analysis/blob/main/Resources/images/ros.png)

- SMOTE

![image](https://github.com/trosie3/Credit_Risk_Analysis/blob/main/Resources/images/SMOTE.png)

- ClusterCentroids

![image](https://github.com/trosie3/Credit_Risk_Analysis/blob/main/Resources/images/cc.png)

- SMOTEENN

![image](https://github.com/trosie3/Credit_Risk_Analysis/blob/main/Resources/images/SMOTEENN.png)

- BalancedRandomForestClassifier

![image](https://github.com/trosie3/Credit_Risk_Analysis/blob/main/Resources/images/balanced_forest.png)

- EasyEnsembleClassifier

![image](https://github.com/trosie3/Credit_Risk_Analysis/blob/main/Resources/images/easy_ensemble.png)

## Summary: 
Of the sampling methods SMOTEENN is the most accurate based on accuracy score alone with a 67.1% however the SMOTE method has the best recall scores and is near SMOTEENN's accuracy score so would be the best of the sampling methods to choose from given both those paramaters. Precision wise all these models are lacking for high-risk and overfit for low-risk. Of the ensemble decision tree methods EasyEnsembleClassifier(EEC) has the better accuracy score, good recall scores, and better f1 scores than the BalancedRandomForestClassifier(BRFC) method, making EEC the better of these two methods. Both still show overfitting for low-risk and poor high-risk precision scores.

Based on these six models and the data given- EEC is the best fit machine learning model assessed given that is has an accuracy score of 93.2%, and good recall(sensitivity) scores for both low- and high-risk predictions with both being over 90%. However with all these models, even EEC, many high-risk people would slip through and high-risk individuals are not good for business in the long run as they are more likely to default. Given the over-fitting all models show in predicting low-risk and the best model only catching 9% of high-risk applicants further analysis is need to truly deterime if EEC is the best model to us to predict credit risk. Thus, my recommendation would be to do further model testing before settling on EEC.
