# Credit Risk Analysis

## Overview of Project

1. Explain how a machine learning algorithm is used in data analytics.
2. Create training and test groups from a given data set.
3. Implement the logistic regression, decision tree, random forest, and support vector machine algorithms.
4. Interpret the results of the logistic regression, decision tree, random forest, and support vector machine algorithms.
5. Compare the advantages and disadvantages of each supervised learning algorithm.
6. Determine which supervised learning algorithm is best used for a given data set or scenario.
7. Use ensemble and resampling techniques to improve model performance.

Software: Python 3.7, NumPy, SciPy, Scikit-learn, SMOTE, SMOTEENN, RandomOverSampler, ClusterCentroids, BalancedRandomForestClassifier, EasyEnsembleClassifier

## Purpose 
Use statistical reasoning and machine learning in order to evaluate credit card risk. The data will come from a credit card dataset from the lending services company, LendingClub. After evaluating this data sample, two different machine learning models will be compared to reduce any bias that may occur when predicting credit risk.  

## Results 

### Deliverable 1 - Resampling Models to Predict Credit Risk
Three machine learning models, RandomOverSamples, SMOTE algorithms, and ClusterCentroids, have been used to evaluate which is better at predicting credit risk. The criteria used for this determination includes balanced accuracy scores, logistic regression classifiers, and classification reports. The resuls for all three can be found below. 

#### RandomOverSampler - Oversampling
![Deliverable_1_RandomOverSampler](https://user-images.githubusercontent.com/88064181/143730265-36c85d52-5143-4a46-93f9-ece1dba2dce8.png)


* Balanced Accuracy Score: 0.6515938052705158
* Precision Score: The precision is low for High-risk loans and is high for Low-risk loans
* Recall Score: 0.62 High Risk/ 0.68 Low Risk
 
#### SMOTE Algorithms - Oversampling
![Deliverable_1_SMOTE_Oversampling](https://user-images.githubusercontent.com/88064181/143730272-7ffeb2a1-8119-4f5f-a8f7-e0f3e43ea983.png)


* Balanced Accuracy Score: 0.6241876870888075
* Precision Score: The precision is low for High-risk loans and is high for Low-risk loans
* Recall Score: 0.59 High Risk/ 0.66 Low Risk

#### ClusterCentroids - Undersampling
![Deliverable_1_Undersampling](https://user-images.githubusercontent.com/88064181/143730280-0d3af227-2045-4665-99ea-b14a7fa9fc5f.png)


* Balanced Accuracy Score: 0.6241876870888075
* Precision Score: The precision is low for High-risk loans and is high for Low-risk loans
* Recall Score: 0.59 High Risk/ 0.43 Low Risk

### Deliverable 2 - SMOTEENN Algorithms to Predict Credit Risk

SMOTEENN algorithms will be used with an over- and under- sampling approach to determine if the results from combinatorial approaches are better at predicting credit risk over the resampling algorithms attempted in deliverable one.

![Deliverable_2_Over_Under_Sampling](https://user-images.githubusercontent.com/88064181/143730283-644839fc-b27b-44e1-ad7e-8c3cce6dcafb.png)


* Balanced Accuracy Score: 0.5103017191018931
* Precision Score: The precision is low for High-risk loans and is high for Low-risk loans
* Recall Score: 0.70 High Risk/ 0.58 Low Risk


### Deliverable 3 - Ensemble Classifiers to Predict Credit Risk

Two different ensemble classifiers, BalancedRandomForestClassifier and EasyEnsemble Classifier, to predict credit risk. 

#### Balanced Random Forest Classifier
![Deliverable_3__Balanced_random_Forest_Classifier](https://user-images.githubusercontent.com/88064181/143730286-a704bcd8-c044-4301-b8f3-b2aca9f574ba.png)


* Balanced Accuracy Score: 0.7877672625306695
* Precision Score: The precision is low for High-risk loans and is high for Low-risk loans.
* Recall Score: 0.67 High Risk/ 0.91 Low Risk

#### Easy Ensemble Classifier
![Deliverable_3__Easy_ensemble](https://user-images.githubusercontent.com/88064181/143730287-58224f90-4bca-4108-be80-04ddca14a744.png)


* Balanced Accuracy Score: 0.9229904850855175
* Precision Score: The precision is low for High-risk loans and is high for Low-risk loans.
* Recall Score: 0.67 High Risk/ 0.91 Low Risk

## Summary
Balanced accuracy uses sensitivity and specificity to evaluate the performance of a classifier. The balanced accuracy is placed on a scale of 0 to 1. The closer to 1 the balanced accurracy is, the better the prediction of the model. For the credit card risk data set, all of the classifiers tested showed similar recall scores, and all had precision scores as low for high-risk loans and high for low-risk loans. The difference in these machine learning models occurs in the balanced accuracy score. The Easy Ensemble Classifier outperformed all off the other models significantly with a score of 0.92. Seeing as none of the other machine learning models had balanced accuracy scores above 0.78, the Easy Ensemble Classifier is the best choice when analyzing and predicting credit card risk. 
 
