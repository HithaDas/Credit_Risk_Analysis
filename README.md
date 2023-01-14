# Credit_Risk_Analysis
Module 18 Credit Risk Analysis


# Background
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we’ll need to employ different techniques to train and evaluate models with unbalanced classes. We have to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. 
Then, we’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Finally, evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

# Overview

In this moduel challenge we have used 6 different imbalanced classifiers, to help make the classifications to see which would work best to classify loan applicants as high risk or low risk. The classifiers used are as follows:

Naive Random Oversampling

SMOTE Oversampling

Undersampling

Combination (Over and Under) Sampling

Balanced Random Forest Classifier

Easy Ensemble AdaBoost Classifier

# Purpose

Create training and test groups from a given data set.
Implement the logistic regression, decision tree, random forest, and support vector machine algorithms.
Interpret the results of the logistic regression, decision tree, random forest, and support vector machine algorithms.
Determine which supervised learning algorithm is best used for the given data set.
Use ensemble and resampling techniques to improve model performance.


# Result

The results for the six machine learning models including their respective balanced accuracy, precision, and recall scores are as follows:

# 1. Naive Random Oversampling

![Naive Random Oversampling](https://user-images.githubusercontent.com/110873947/212485673-a976b147-bf79-432c-8c82-a82147b31cc0.png)

accuracy score: 0.6556397581090282

precision score: (high risk: 0.01)(low risk: 1.00)(avg/total: 0.99)

recall score: (high risk: 0.64)(low risk: 0.67)(avg/total: 0.67)

# 2. SMOTE Oversampling

![SMOTE Oversampling](https://user-images.githubusercontent.com/110873947/212485755-471a237d-963b-4770-80be-0220028b94e4.png)


accuracy score: 0.6642715270475523

precision score: (high risk: 0.01)(low risk: 1.00)(avg/total: 0.99)

recall score: (high risk: 0.67)(low risk: 0.66)(avg/total: 0.66)

# 3. Undersampling

![Undersampling](https://user-images.githubusercontent.com/110873947/212485827-3c11c7eb-f7ed-44dc-ad76-e1924382cbbd.png)


Balanced Accuracy: 0.6642715270475523
Precision: (high risk: 0.01)(low risk: 1.00)(avg/total: 0.99).
Recall: (high risk: 0.61)(low risk: 0.45)(avg/total: 0.45)

# 4. Combination (Over and Under) Sampling

![Combination Under-Over Sampling](https://user-images.githubusercontent.com/110873947/212485929-46aa22ac-7701-44bf-82e5-5214dabc3f50.png)

Balanced Accuracy: 0.5293318990697431
Precision: (high risk: 0.01)(low risk: 1.00)(avg/total: 0.99).
Recall: (high risk: 0.70)(low risk: 0.57)(avg/total: 0.57)


# 5. Balanced Random Forest Classifier

![Balanced Random Forest Classifier](https://user-images.githubusercontent.com/110873947/212486255-fa63009a-a086-4dc6-826c-302daa30a92d.png)


Balanced Accuracy: 0.7887512850910909
Precision: (high risk: 0.01)(low risk: 0.00)(avg/total: 0.00).
Recall: (high risk: 1)(low risk: 0.00)(avg/total: 0.01)


# 6. Easy Ensemle AdaBoost Classifier

![Easy Ensemble AdaBoost Classifier](https://user-images.githubusercontent.com/110873947/212486792-806578a7-5d7a-48e5-8b3b-d94bf3a6e314.png)


Balanced Accuracy: 0.9316600714093861
Precision: (high risk: 0.09)(low risk: 1.00)(avg/total: 0.99).
Recall: (high risk: 0.92)(low risk: 0.94)(avg/total: 0.94)

# Summary

The classifiers seem to be have a relatively similar accuracy and within appropriate ranges,
other than the Easy Ensemble AdaBoost Classifier. 
When working with balanced accuracy, the highest compared accuracy between 0 and 1 and is closest to 1 is the best machine learning model. 
For the present credit card data set, the Easy Ensemble AdaBoost Classifier is the best model to choose with its .93 balanced accuracy.
Easy Ensemble AdBoost Classifier has a low precision score for high risk, the precision is still higher than all of the other classifiers. The Easy Ensemble AdaBoost Classifier had the highest recall score, making it the final best machine learning model to choose for further credit card analysis.


