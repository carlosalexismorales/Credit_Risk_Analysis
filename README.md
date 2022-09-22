# Credit_Risk_Analysis


## Project Overview

In this analysis, Machine Learning statistical algorithms are used to make predictions and find patterns from a database. This type of Machine Learning is Supervised because the data has labeled outcomes that we used. This analysis uses a dataset from LendingClub to predict credit and loan risk - this will help the company make better decisions when they are evaluating potiential borrowers since credit risk is an inherently unbalanced classification problem, as good loans  outnumber risky loans. 

In order to get the most accurate predictions, we use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. We also oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Finally, we evaluate the performance of these models. 


## Challenge Overview

1. Use Resampling Models to Predict Credit Risk
2. Use the SMOTEENN Algorithm to Predict Credit Risk
3. Use Ensemble Classifiers to Predict Credit Risk


## Results


### Splitting Data into Testing and Training 

In the images below, we use Machine Learning to resample the dataset using Python libraries: scikit-learn and imbalanced-learn evaluate the results and provide a comparison for our analysis. We use 'loan_status' as the target value to determine 'low risk' or 'high risk'. Then, the data is split into testing and training sets. We see the data split for training vs. testing sets with 51,366 'low risk' and 246 'high risk' applications were categorized into the training set and 17,104 'low' risk and 101 'high' risk applications into testing. 




<img width="1007" alt="Screen Shot 2022-09-21 at 8 37 15 PM" src="https://user-images.githubusercontent.com/102444078/191652937-3b19a5ee-ee04-479b-b01b-31d9148bbb4b.png">




<img width="1012" alt="Screen Shot 2022-09-21 at 8 40 29 PM" src="https://user-images.githubusercontent.com/102444078/191653281-c4d5dd05-6cf2-4a16-887a-b3698f78faf4.png">





### Oversampling

In this part of the analysis, we compare two oversampling algorithms to determine which algorithm results in the best performance. We oversample the data using the naive random oversampling algorithm and the SMOTE algorithm.






#### Naive Random Oversampling 

We see the following in the images below: 

- With the naive random oversampling algorithm, we see the results classified 51,366 records each as 'High Risk' and 'Low Risk'. 
- Balanced accuracy score: 67%
- The 'High Risk' precision rate was only 1% with the recall at 74% giving this model an F1 score of 2%.
- The 'Low Risk' had a precision rate of 100% and recall at 61% giving this model an F1 score of 75%




<img width="1012" alt="Screen Shot 2022-09-21 at 8 46 07 PM" src="https://user-images.githubusercontent.com/102444078/191653905-af7d65e2-4481-400b-ad12-ccef25322f44.png">



<img width="1022" alt="Screen Shot 2022-09-21 at 8 46 23 PM" src="https://user-images.githubusercontent.com/102444078/191653944-8a87b9f3-dc11-4a21-9f87-e2b358621372.png">




<img width="1004" alt="Screen Shot 2022-09-21 at 8 46 47 PM" src="https://user-images.githubusercontent.com/102444078/191653988-3002b5db-d729-4ead-a18e-1bbaf0431944.png">





#### Smote Oversampling 




### Undersampling 


In this part of the analysis, we test an undersampling algorithms to determine which algorithm results in the best performance compared to the oversampling algorithms above. We undersample the data using the Cluster Centroids algorithm. 







### Combination (Over and Under Sampling)

In this part of the analysis, we test a combination over- and under-sampling algorithm to determine if the algorithm results in the best performance compared to the other sampling algorithms above. We resample the data using the SMOTEENN algorithm.














 
## Summary 

