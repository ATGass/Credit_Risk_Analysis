# Credit_Risk_Analysis
## Overview
The idea behind this analysis is to try out different machine learning techniques and choose the best one to understand and interpret credit risk. We will classify the potential credit users as either high-risk or low-risk. We will determine which model best predicts the type of credit user depending on the various data points within LendingClub's dataset.

## Results
### RandomOverSampler
* Accuracy Score: 64.98%
* Classification Report: 
<img width="599" alt="RandomOverSampler" src="https://user-images.githubusercontent.com/82982180/136480324-17df75ca-d344-4596-8d69-3e5aeaa0f0c0.png">

### SMOTE
* Accuracy Score: 64.44%
* Classification Report:
<img width="599" alt="SMOTE" src="https://user-images.githubusercontent.com/82982180/136480619-fe0cae7c-cfb1-490e-a17a-77e71bb4a02e.png">

### ClusterCentroids
* Accuracy Score: 64.44%
* Classification Report: 
<img width="599" alt="ClusterCentroids" src="https://user-images.githubusercontent.com/82982180/136481280-e71a37e4-39cc-4272-8296-dee0b223d031.png">

### SMOTEENN
* Accuracy Score: 59.55%
* Classification Report:
<img width="599" alt="SMOTEENN" src="https://user-images.githubusercontent.com/82982180/136481070-1501d05f-3705-4535-a0ea-b57836f8b5b6.png">

### BalancedRandomForestClassifier
* Accuracy Score: 49.66%
* Classification Report: 
<img width="599" alt="BalancedRandomForrest" src="https://user-images.githubusercontent.com/82982180/136480918-fec89064-7f2d-4e98-84f4-623ff148a83e.png">

### EasyEnsembleClassifier
* Accuracy Score: 92.43%
* Classification Report: 
<img width="599" alt="EasyEnsembleClassifier" src="https://user-images.githubusercontent.com/82982180/136480798-0207867b-d1ae-47fe-a003-e504ef4b30cd.png">

## Summary
EasyEnsemleClassifier has the best accuracy score of any model. It has a terrible overall f1 score along with BalancedRandomForestClassifier. All the other models have an overall f1 score of 72 or better which is decent, but all of their f1 scores are .02 or worse for users that are considered to be "high risk". Since no model does a good job of predicting potential high risk customers I do not recommend any model. It is a problem if we are not able to identify those who are high risk.
