# Module 18 Challenge: Credit_Risk_Analysis

## Overview of the analysis:
   Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans.  In an attempt to resolve the class imbalance, we will use the credit card credit dataset from LendingClub, a peer-to-peer lending services company, to oversample the data using the RandomOverSampler and SMOTE algorithms, undersample the data using the ClusterCentroids algorithm and finally, use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. We will then compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Upon completion, we will evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.


## Results:
#### RandomOverSampler Resampling Model WITH Logistic Regression Classifier:
- Balanced Accuracy Score: 0.661 = ~66% accurate overall
- Precision Score:  High Risk - 0.01,  Low Risk - 1.00
- Recall Score:  High Risk - 0.72,   Low Risk - 0.60

![image](https://user-images.githubusercontent.com/114360511/218954527-4f9b79e1-0ebc-4c1e-84f6-8d9175782a7f.png)

#### SMOTE Resampling Model WITH Logistic Regression Classifier:
- Balanced Accuracy Score: 0.658 = ~66% accurate overall
- Precision Score:  High Risk - 0.01,  Low Risk - 1.00
- Recall Score:  High Risk - 0.62,   Low Risk - 0.69

![image](https://user-images.githubusercontent.com/114360511/218954638-d4f03cc1-df46-4a62-a512-99b9690850d5.png)

#### ClusterCentroids Resampling Model WITH Logistic Regression Classifier:
- Balanced Accuracy Score: 0.545 = ~55% accurate overall
- Precision Score:  High Risk - 0.01,  Low Risk - 1.00
- Recall Score:  High Risk - 0.69,   Low Risk - 0.40

![image](https://user-images.githubusercontent.com/114360511/218954325-805e791b-3df2-4594-aa8f-00a691a94faa.png)

#### SMOTEENN Resampling Model WITH Logistic Regression Classifier:
- Balanced Accuracy Score: 0.671 = ~67% accurate overall
- Precision Score:  High Risk - 0.01,  Low Risk - 1.00
- Recall Score:  High Risk - 0.77,   Low Risk - 0.57

![image](https://user-images.githubusercontent.com/114360511/218954592-f19c2304-02b9-4b85-8e9e-02b1582e3d28.png)

#### BalancedRandomForestClassifier Machine Learning Model:
- Balanced Accuracy Score: 0.789 = ~79% accurate overall
- Precision Score:  High Risk - 0.03,  Low Risk - 1.00
- Recall Score:  High Risk - 0.70,   Low Risk - 0.87

![image](https://user-images.githubusercontent.com/114360511/218954294-0a43f395-d746-4015-8879-ebf503488829.png)

#### EasyEnsembleClassifier Machine Learning Model:
- Balanced Accuracy Score: 0.932 = ~93% accurate overall
- Precision Score:  High Risk - 0.09,  Low Risk - 1.00
- Recall Score:  High Risk - 0.92,   Low Risk - 0.94

![image](https://user-images.githubusercontent.com/114360511/218954416-07cdd5e8-243a-46b2-a345-05ed95009149.png)


## Summary: 
In summary, the overall accuracy scores for using the Logistic Regression classifier with resampling of the classes produced only moderate scores(55%- 67%), while the use of the two new ensemble machine learning models resulted in better scores(79% and 93%).  Thus showing that our attempts to rebalance the classes resulted in only modest accuracy scores.

For precision scores, all methods (both resampling and new models) showed the same results. As far as predicting high credit risk, all models showed no precision (0.1 - 0.09), meaning far too many false positive (type I error) results.  On the flip side, when predicting for low credit risk and models were perfect, meaning very few false negatives.  So if being right when predicting low risk is important and predicting correctly for high risk doesnt matter, these models are good, but otherwise they fail.

For recall scores, most high credit risk and low credit risk scores fell between 0.57 and 0.77, with a few notable exceptions.  On the low end the Cluster Centroids Resampling method had a low score of 0.40 for low credit risk and the Balanced Random Forest model had a relatively high score of 0.87 for low credit risk.  The one standout overall for recall was the Easy Ensemble Classifier model with 0.92 for high credit risk and 0.94 for low credit risk.

For recommendations, if accurate predictions of high risk credit with little room for type I errors (false positives) is important, I can't recommend any of these models as they all show no precision.  If accurate predictions of high risk credit with a little room for type II errors (false negatives) is important, then we would recommend using the Easy Ensemble Classifier model without resampling, as it scored an impressive 0.92 recall with an overall accuracy score of 93%.
If accurate predictions of low risk credit with little room for type I errors (false positives) is important, all models succeeded with precison scores of 1.0, but again I would recommend the Easy Ensemble Classifier model without resampling, as it also provided very high recall scores.  Finally, if accurate predictions of low risk credit with a little room for type II errors (false negatives) is important, then we would recommend using the Easy Ensemble Classifier model without resampling, as it scored an impressive 0.94 recall, as well as high scores(0.92) on low credit risk precision.







