# Credit_Risk_Analysis
## Overview
Good loans far exceed dangerous loans, credit risk can be difficult to classify. It's common to use machine learning models to predict the risk of a loan. In order to use machine learning predictive models, the sample size of risky loans must be changed to balance out the data with the rest of the safe loans. 
We evaluated a loans dataset from the Lending Club's first quarter of 2019 with four different re-sampling methods using "imbalanced-learn" and "scikit-learn" python libraries to determine its accuracy. We also compared two machine-learning models to compare their credit risk prediction performance. 


## Results

Random Over Sampler
* The random oversampling method got an accuracy score of 62.3%, a precision score of 1%, and a recall/sensitivity score of 57%.

SMOTE sampler
* The Synthetic Minority Oversampling Technique got an accuracy score of 62.8%, a precision score of 1%, and a recall/sensitivity score of 62%.

Cluster Centroids under-sampler
* The undersampling method got an accuracy score of 62.8%, a precision score of 1%, and a recall/sensitivity score of 59%.

SMOTE-ENN sampler
* The SMOTE combined with Edited Nearest Neighbor (ENN) technique of over and undersampling mixed method got an accuracy score of 78.9%, a precision score of 3%, and a recall/sensitivity score of 70%.

Balanced Forest Classifier model
* The random forest algorithm got an accuracy score of 62.8%, a precision score of 1%, and a recall/sensitivity score of 59%.

Easy Ensemble Classifier model
* The adaptive boosting model got an accuracy score of 93.2%, a precision score of 9%, and a recall/sensitivity score of 92%.

## Summary

Most of the re-sampling models showed a very small difference in accuracy. The SMOTE-ENN combination of sampling was the only model to have a significant difference of 78% accuracy compared to under 63% scores of the other three sampling methods. Although all the models have a very low precision score, the SMOTE-ENN method still had a higher precision of 6%. 

Between both predictive models, the Easy Ensemble classifier is much better at predicting credit risk. This method has higher scores all around compared to the Balanced Forest Classifier. I would recommend banks to use the Easy Ensemble Classifier model for credit risk. 
