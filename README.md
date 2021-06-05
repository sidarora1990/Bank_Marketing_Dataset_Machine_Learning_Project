# Bank Marketing Dataset Machine Learning Project
## The Task
The "Bank Marketing Data Set" from the UCI Machine Learning Repository is related with direct marketing campaigns (phone calls) of a Portuguese banking institution.

The classification goal is to predict if the client will subscribe a term deposit (variable y). You can find a description of the attributes at the original UCI URL, https://archive.ics.uci.edu/ml/datasets/Bank+Marketing.
In this project we build two classifiers for this data set: a decision tree, and a random forest. We use ROC AUC score as an evaluation metric to compare the performance of the two classifiers.
## Approach
<ul>
  <li> We devise two feature engineering appraoches: First, Label encoding of Education and One-hot encoding of categorical fields and second, ordinal encoding of Education and One-hot encoding of categorical fields</li>
  <li>Create pipeline of Feaure Engineering and the ML model i.e. Decision Tree or Random Forest.</li>
  </ul>
  
 ## Pipeline
 <p>Pipelines are useful in designing a flow of events to be executed. The main purpose of this project is to show the use of Sklearn's pipeline to execute stratified K fold cross validation,feature engineering and fit a machine learning model in this specific order. Stratified K fold cross validation is used to tackle over-fitting. We calculate the mean train score and test score for each classifier.</p>  
 <p> We also use SMOTE and undersampling as two further steps in the pipline to tackle the class imabalnce of the data. We randomly undersample 50% of the data pertaining to majority class and oversample 20% of the data pertaining to minority class. In this way, we decrease the class imbalance to a larger extent if not zero. The usage of both oversampling of minority class and undersampling of majority class ensures better result than either of the methods used.</p>
<p> After fitting the pipeline for random forest, we collect the important features for each of the 10 estimators (since 10-fold stratified cross validation) and store them in a dataframe in decreasing order of importance. Based on the most important features, we can fit the model again and recompute the train and test accuracy.</p>

## Results
<p>We observe that Random forest with 50 estimators outperforms Decision trees and Random Forest with SMOTE and Random Undersampling combination.</p>
