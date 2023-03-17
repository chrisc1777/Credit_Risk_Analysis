# Credit_Risk_Analysis
## Overview
Good loans far exceed dangerous loans, credit risk can be difficult to classify. It's common to use machine learning models to predict the risk of a loan. In order to use machine learning predictive models, the sample size of risky loans must be changed to balance out the data with the rest of the safe loans. 
We evaluated a loans dataset from the Lending Club's first quarter of 2019 with four different re-sampling methods using "imbalanced-learn" and "scikit-learn" python libraries to determine its accuracy. We also compared two machine-learning models to compare their credit risk prediction performance. 


## Results

Random Over Sampler
* The random oversampling method got an accuracy score of 62.3%, a precision score of 1%, and a recall/sensitivity score of 57%.
![nro](https://user-images.githubusercontent.com/106359564/225806153-3cfc3196-22f3-44a1-a300-8b9a9a21e63d.png)


SMOTE sampler
* The Synthetic Minority Oversampling Technique got an accuracy score of 62.8%, a precision score of 1%, and a recall/sensitivity score of 62%.
![smote](https://user-images.githubusercontent.com/106359564/225806183-614039ff-d903-46d4-982e-b32b45227ca3.png)


Cluster Centroids under-sampler
* The undersampling method got an accuracy score of 62.8%, a precision score of 1%, and a recall/sensitivity score of 59%.
![under](https://user-images.githubusercontent.com/106359564/225806217-ead77bf3-3538-4c6b-b48b-4b800cce1597.png)


SMOTE-ENN sampler
* The SMOTE combined with Edited Nearest Neighbor (ENN) technique of over and undersampling mixed method got an accuracy score of 78.9%, a precision score of 3%, and a recall/sensitivity score of 70%.
![smoteenn](https://user-images.githubusercontent.com/106359564/225806235-b1d8759a-9204-4e3e-b032-cf4c7610ec6a.png)


Balanced Forest Classifier model
* The random forest algorithm got an accuracy score of 62.8%, a precision score of 1%, and a recall/sensitivity score of 59%.
![forest](https://user-images.githubusercontent.com/106359564/225806257-645cc06d-2264-4514-9326-031af02fa09a.png)


Easy Ensemble Classifier model
* The adaptive boosting model got an accuracy score of 93.2%, a precision score of 9%, and a recall/sensitivity score of 92%.
![adaboost](https://user-images.githubusercontent.com/106359564/225806272-b21a6449-a6e0-4c4b-8f08-54514afa0085.png)


## Summary

Most of the re-sampling models showed a very small difference in accuracy. The SMOTE-ENN combination of sampling was the only model to have a significant difference of 78% accuracy compared to under 63% scores of the other three sampling methods. Although all the models have a very low precision score, the SMOTE-ENN method still had a higher precision of 6%. 

Between both predictive models, the Easy Ensemble classifier is much better at predicting credit risk. This method has higher scores all around compared to the Balanced Forest Classifier. I would recommend banks to use the Easy Ensemble Classifier model for credit risk. 
