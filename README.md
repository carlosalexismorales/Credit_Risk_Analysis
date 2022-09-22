# Credit_Risk_Analysis


## Project Overview

In this analysis, Machine Learning statistical algorithms are used to make predictions and find patterns from a database. This type of Machine Learning is Supervised because the data has labeled outcomes that we used. This analysis uses a dataset from LendingClub to predict credit and loan risk - this will help the company make better decisions when they are evaluating potiential borrowers since credit risk is an inherently unbalanced classification problem, as good loans  outnumber risky loans. Therefore, in order to get the most accurate predictions, we use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. We also oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Finally, we evaluate the performance of these models. 


## Challenge Overview

1. Use Resampling Models to Predict Credit Risk
2. Use the SMOTEENN Algorithm to Predict Credit Risk
3. Use Ensemble Classifiers to Predict Credit Risk


## Results

### Splitting Data into Testing and Training 

In the images below, we use Machine Learning to resample the dataset using Python libraries: scikit-learn and imbalanced-learn evaluate the results and provide a comparison for our analysis. We use 'loan_status' as the target value to determine 'low' or 'high' risk. Then, the data is split into testing and training sets.









### Oversampling

In this part of the analysis, we compare two oversampling algorithms to determine which algorithm results in the best performance. We oversample the data using the naive random oversampling algorithm and the SMOTE algorithm.






#### Naive Random Oversampling 








#### Smote Oversampling 




### Undersampling 


In this part of the analysis, we test an undersampling algorithms to determine which algorithm results in the best performance compared to the oversampling algorithms above. We undersample the data using the Cluster Centroids algorithm. 







### Combination (Over and Under Sampling)

In this part of the analysis, we test a combination over- and under-sampling algorithm to determine if the algorithm results in the best performance compared to the other sampling algorithms above. We resample the data using the SMOTEENN algorithm.














 
## Summary 

