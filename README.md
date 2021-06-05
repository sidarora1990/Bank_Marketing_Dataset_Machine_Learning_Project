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
 <p>Pipelines are usefull in designing a flow of events to be executed. The main purpose of this project is to show the use of Sklearn's pipeline to execute stratified K fold cross validation,feature engineering , machine learning model in this specific order. Stratified k fold cross validation is used to counter over-fitting.</p>  

