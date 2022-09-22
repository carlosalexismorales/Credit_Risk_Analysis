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
- The 'High Risk' precision rate was 1% with the recall at 74% giving this model an F1 score of 2%.
- The 'Low Risk' had a precision rate of 100% and recall at 61% giving this model an F1 score of 75%




<img width="1012" alt="Screen Shot 2022-09-21 at 8 46 07 PM" src="https://user-images.githubusercontent.com/102444078/191653905-af7d65e2-4481-400b-ad12-ccef25322f44.png">



<img width="1022" alt="Screen Shot 2022-09-21 at 8 46 23 PM" src="https://user-images.githubusercontent.com/102444078/191653944-8a87b9f3-dc11-4a21-9f87-e2b358621372.png">




<img width="1004" alt="Screen Shot 2022-09-21 at 8 46 47 PM" src="https://user-images.githubusercontent.com/102444078/191653988-3002b5db-d729-4ead-a18e-1bbaf0431944.png">





#### Smote Oversampling 


In the images below, we see the following: 

- Balanced accuracy score: 66%
- The 'High Risk' had a precision rate of 1% with the recall at 63% giving this model an F1 score of 2%.
- The 'Low Risk' had a precision rate of 100% and recall at 69% giving this model an F1 score of 82%



<img width="1007" alt="Screen Shot 2022-09-21 at 9 02 41 PM" src="https://user-images.githubusercontent.com/102444078/191655806-253360bb-9df8-47ab-8bf6-13e6f0df6d5e.png">



<img width="1017" alt="Screen Shot 2022-09-21 at 9 03 00 PM" src="https://user-images.githubusercontent.com/102444078/191655835-6846dd2d-9c49-4e17-b5ae-e939dc0d2e65.png">











### Undersampling 


In this part of the analysis, we test an undersampling algorithms to determine which algorithm results in the best performance compared to the oversampling algorithms above. We undersample the data using the Cluster Centroids algorithm. 


In the images below, we see the following:

- Balanced accuracy score: 54%
- The 'High Risk' had a precision rate of 1% with the recall at 69% giving this model an F1 score of 1%.
- The 'Low Risk' had a precision rate of 100% and recall at 40% giving this model an F1 score of 57%


<img width="1015" alt="Screen Shot 2022-09-21 at 9 08 02 PM" src="https://user-images.githubusercontent.com/102444078/191656342-cb644833-df25-4f8a-b78a-75ed6688db96.png">






<img width="1014" alt="Screen Shot 2022-09-21 at 9 08 22 PM" src="https://user-images.githubusercontent.com/102444078/191656389-62677e12-b407-4e9b-9116-9b2d0db02e46.png">







### Combination (Over and Under Sampling)

In this part of the analysis, we test a combination over- and under-sampling algorithm to determine if the algorithm results in the best performance compared to the other sampling algorithms above. We resample the data using the SMOTEENN algorithm.


We see the following in the images below:

- Balanced accuracy score: 65%
- The 'High Risk' had a precision rate of 1% with the recall at 72% giving this model an F1 score of 2%.
- The 'Low Risk' had a precision rate of 100% and recall at 57% giving this model an F1 score of 72%


<img width="1010" alt="Screen Shot 2022-09-21 at 9 12 01 PM" src="https://user-images.githubusercontent.com/102444078/191656792-0c6581b8-be04-4bc6-a330-4df5b33fac5d.png">




<img width="1014" alt="Screen Shot 2022-09-21 at 9 12 24 PM" src="https://user-images.githubusercontent.com/102444078/191656829-5706ba3d-df24-4862-8102-1e45d8a5ecdd.png">


### Ensemble Learners

In this part of the analysis, we compare two ensemble algorithms to determine which algorithm results in the best performance. We train a Balanced Random Forest Classifier and an Easy Ensemble AdaBoost classifier

#### Balanced Forest Classifier

We see the following in the images below:

- Balanced accuracy score: 79%
- The 'High Risk' had a precision rate of 3% with the recall at 70% giving this model an F1 score of 6%.
- The 'Low Risk' had a precision rate of 100% and recall at 87% giving this model an F1 score of 93%


<img width="1008" alt="Screen Shot 2022-09-21 at 9 17 10 PM" src="https://user-images.githubusercontent.com/102444078/191657375-ebea0015-0976-488f-a999-f195eaff8e32.png">




<img width="1029" alt="Screen Shot 2022-09-21 at 9 17 29 PM" src="https://user-images.githubusercontent.com/102444078/191657411-422885b0-9e63-43a2-a7fa-b9bf56e697c8.png">



<img width="1029" alt="Screen Shot 2022-09-21 at 9 18 07 PM" src="https://user-images.githubusercontent.com/102444078/191657466-a5b3baa0-7e72-428d-b261-5d337142c652.png">


#### Easy Ensemble AdaBoost Classifier


We see the following in the images below:

- Balanced accuracy score: 93%
- The 'High Risk' had a precision rate of 9% with the recall at 92% giving this model an F1 score of 16%.
- The 'Low Risk' had a precision rate of 100% and recall at 94% giving this model an F1 score of 97%


<img width="1008" alt="Screen Shot 2022-09-21 at 9 20 30 PM" src="https://user-images.githubusercontent.com/102444078/191657710-0f6a1fcb-d997-4610-a9ed-b12a5acd6ada.png">




<img width="1010" alt="Screen Shot 2022-09-21 at 9 21 15 PM" src="https://user-images.githubusercontent.com/102444078/191657796-cf4f5fd4-1edc-475a-ab5a-506040bf20a0.png">






 
## Summary 

