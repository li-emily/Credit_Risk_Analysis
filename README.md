# Credit_Risk_Analysis


## Overview
### Purpose 
>Apply machine learning to solve a real-world challenge: credit card risk. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. 

- Use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.
- Oversample data with RandomOverSampler, and SMOTE algorithms.
- Undersample data using ClusterCentroids algorithm.
- Combination sampling (over + under) using SMOTEENN algorithm.
- Compare new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier.
- Evaluate model performance and determine the most well suited for further predictions.

### Resources
- Languages and Packages: Python, pandas, numpy, imbalanced-learn, scikit-learn, path, collections
- Interface and Environment: Jupyter Notebook, Visual Studio Code, Terminal, Miniconda
- Data Source: Credit card credit dataset from LendingClub

## Results
### Deliverable 1
Naive Random Oversampling: Balanced accuracy score: 64.9%. Recall (sensitivity) is at 68% overall.
![](https://raw.githubusercontent.com/li-emily/Credit_Risk_Analysis/main/Resources/d1-naive-random-oversampling.png)

SMOTE Oversampling: Balanced accuracy score: 64.4%. Recall is at 66% overall.

![](https://raw.githubusercontent.com/li-emily/Credit_Risk_Analysis/main/Resources/d1-smote-oversampling.png)

Undersampling: Balanced accuracy is at 64.4%. Recall rate is 45% overall.

![](https://raw.githubusercontent.com/li-emily/Credit_Risk_Analysis/main/Resources/d1-undersampling.png)

### Deliverable 2
Combination Sampling - SMOTEENN: Balanced accuracy is 52.9%, and recall rate is 57% overall. 

![](https://raw.githubusercontent.com/li-emily/Credit_Risk_Analysis/main/Resources/d2-combination-smoteenn.png)

### Deliverable 3
Balanced Random Forest Classifier: Balanced accuracy is 99.9%. Recall/sensitivity is 100%.

![](https://raw.githubusercontent.com/li-emily/Credit_Risk_Analysis/main/Resources/d3-balanced-random-forest.png)

Easy Ensemble Classifier: Balanced accuracy is at 100%, and recall is 100%.
![](https://raw.githubusercontent.com/li-emily/Credit_Risk_Analysis/main/Resources/d3-easy-ensemble.png)

## Summary
For the first portion, we oversampled twice, undersampled, and combination sampled to predict credit risk. Accuracy score ranged in the 50-60s percent. These four models did use all of the variables. For second portion, we resampled the data using balanced random forest and easy ensemble classifiers after choosing which variables to use in the model. Accuracy for the two was much higher, close to 100%, and sensitivity/recall was also 100%.
It seems that Easy Ensemble Classifier would be the best model to use, with the best balance of accuracy, precision, and sensitivity.