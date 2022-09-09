# Credit_Risk_Analysis

## Overview of Analysis

Using the unbalanced LendingClub credit card dataset we looked to evaluate different machine learning models. The models used in this analysis were:
 - RandomOverSampler
 - SMOTE
 - ClusterCentroids
 - SMOTEENN
 - BalancedRandomForestClassifier
 - EasyEnsembleClassifier

### Purpose

The purpose of this analysis was to look at the performance for each model and recommend whether they should ve used to predict credit risk.

## Results

The notebooks where this analysis was performed are listed below:

[credit_risk_resampling.ipynb](https://github.com/ClaudAMC/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb)

[credit_risk_ensemble.ipynb](https://github.com/ClaudAMC/Credit_Risk_Analysis/blob/main/credit_risk_ensemble.ipynb)

The results for each of the models evaluated are found below.

### 1. RandomOverSampler

      a. Balanced Accuray: 67.4%
      
      b. Precision: 1%
      
      c. Recall: 71%
      
![RandomOverSampler - BA.PNG](https://github.com/ClaudAMC/Credit_Risk_Analysis/blob/main/Resources/Images/RandomOverSampler%20-%20BA.PNG)
      
![RandomOverSampler - CReport.PNG](https://github.com/ClaudAMC/Credit_Risk_Analysis/blob/main/Resources/Images/RandomOverSampler%20-%20CReport.PNG)   

### 2. SMOTE

      a. Balanced Accuray: 66.2%
      
      b. Precision: 1%
      
      c. Recall: 63%
      
![SMOTE - BA.PNG](https://github.com/ClaudAMC/Credit_Risk_Analysis/blob/main/Resources/Images/SMOTE%20-%20BA.PNG)

![SMOTE - CReport.PNG](https://github.com/ClaudAMC/Credit_Risk_Analysis/blob/main/Resources/Images/SMOTE%20-%20CReport.PNG)

### 3. ClusterCentroids

      a. Balanced Accuray: 54.4%
      
      b. Precision: 1%
      
      c. Recall: 69%

![ClusterCentroids - BA.PNG](https://github.com/ClaudAMC/Credit_Risk_Analysis/blob/main/Resources/Images/ClusterCentroids%20-%20BA.PNG)

![ClusterCentroids - CReport.PNG](https://github.com/ClaudAMC/Credit_Risk_Analysis/blob/main/Resources/Images/ClusterCentroids%20-%20CReport.PNG)

### 4. SMOTEENN

      a. Balanced Accuray: 64.6%
      
      b. Precision: 1%
       
      c. Recall: 72%

![SMOTEENN - BA.PNG](https://github.com/ClaudAMC/Credit_Risk_Analysis/blob/main/Resources/Images/SMOTEENN%20-%20BA.PNG)

![SMOTEENN - CReport.PNG](https://github.com/ClaudAMC/Credit_Risk_Analysis/blob/main/Resources/Images/SMOTEENN%20-%20CReport.PNG)

### 5. BalancedRandomForestClassifier

      a. Balanced Accuray: 78.9%
      
      b. Precision: 3%
      
      c. Recall: 70%

![BalancedRandomForestClassifier - BA.PNG](https://github.com/ClaudAMC/Credit_Risk_Analysis/blob/main/Resources/Images/BalancedRandomForestClassifier%20-%20BA.PNG)

![BalancedRandomForestClassifier - CReport.PNG](https://github.com/ClaudAMC/Credit_Risk_Analysis/blob/main/Resources/Images/BalancedRandomForestClassifier%20-%20CReport.PNG)

### 6. EasyEnsembleClassifier

      a. Balanced Accuray: 93.2%
      
      b. Precision: 9%
      
      c. Recall: 92%

![EasyEnsembleClassifier - BA.PNG](https://github.com/ClaudAMC/Credit_Risk_Analysis/blob/main/Resources/Images/EasyEnsembleClassifier%20-%20BA.PNG)

![EasyEnsembleClassifier - CReport.PNG](https://github.com/ClaudAMC/Credit_Risk_Analysis/blob/main/Resources/Images/EasyEnsembleClassifier%20-%20CReport.PNG)

## Summary

Overall, all models had a low precision score with the highest precision being 9% from the EasyEnsembleClassifier Model.
This model also had the highest balanced accuracy score at 93.2%. Additionally, this model also had the highest recall at 92%, making it the most sensative model. These results point towards this model being the best out of the ones evaluated here and therefore my most recommended out of the ones avaliable. However, I can not completely recommend this model. The high recall percentage means that it will likely be able to catch most fraud cases but the very low precision score means that it will likely also catch many non-fraud cases and classify them as fraud. This may not matter too much to credit companies as non-fraud cases may be easily verifiable; if this is the case then the EasyEnsembleClassifier model would be the one I recommend the most.
