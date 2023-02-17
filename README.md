# Module 18 Challenge: Credit_Risk_Analysis

## Overview of the analysis:
   Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans.  In an attempt to resolve the class imbalance, we will use the credit card credit dataset from LendingClub, a peer-to-peer lending services company, to oversample the data using the RandomOverSampler and SMOTE algorithms, undersample the data using the ClusterCentroids algorithm and finally, use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. We will then compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Upon completion, we will evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.


## Results:

    Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

    There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models (15 pt)

#### RandomOverSampler Resampling Model WITH Logistic Regression Classifier:
- Balanced Accuracy Score:
- Precision Score:
- Recall Score:

![image](https://user-images.githubusercontent.com/114360511/218954527-4f9b79e1-0ebc-4c1e-84f6-8d9175782a7f.png)

#### SMOTE Resampling Model WITH Logistic Regression Classifier:
- Balanced Accuracy Score:
- Precision Score:
- Recall Score:

![image](https://user-images.githubusercontent.com/114360511/218954638-d4f03cc1-df46-4a62-a512-99b9690850d5.png)

#### ClusterCentroids Resampling Model WITH Logistic Regression Classifier:
- Balanced Accuracy Score:
- Precision Score:
- Recall Score:

![image](https://user-images.githubusercontent.com/114360511/218954325-805e791b-3df2-4594-aa8f-00a691a94faa.png)

#### SMOTEENN Resampling ModelWITH Logistic Regression Classifier:
- Balanced Accuracy Score:
- Precision Score:
- Recall Score:

![image](https://user-images.githubusercontent.com/114360511/218954592-f19c2304-02b9-4b85-8e9e-02b1582e3d28.png)

#### BalancedRandomForestClassifier Machine Learning Model:
- Balanced Accuracy Score:
- Precision Score:
- Recall Score:

![image](https://user-images.githubusercontent.com/114360511/218954294-0a43f395-d746-4015-8879-ebf503488829.png)

#### EasyEnsembleClassifier Machine Learning Model:
- Balanced Accuracy Score:
- Precision Score:
- Recall Score:

![image](https://user-images.githubusercontent.com/114360511/218954416-07cdd5e8-243a-46b2-a345-05ed95009149.png)


## Summary: 

    Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

- There is a summary of the results (2 pt)
- There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)
