# Employee-Attrition
# Objective
Prediction of employee attrition with the help of machine learning models like KNN classifier and decision Tree
# About the dataset
The dataset was downloaded from Kaggle. It has around 1470 records. Attrition is our target variable in the dataset.
# Data pre-processing and feature selection
There were no null values in the dataset. Some of the features like EmployeeCount, EmployeeNumber, over18 do not contribute much to the efficiency of the models so were dropped from the datset. Pandas get_dummies function is used to enode the categorical variables. MinMax scaler is used to scale the data between 0 and 1.
# Methodology and conclusions
Using KNeighborsClassifier and cross validation where cv equal to 5 we got a validation accuracy of 84.89 % at k = 8 


Using KNeighborsClassifier and train test split we got a testing accuracy of  85.03 percent at K = 9


Using DecisionTreeClassifier and train test split we got a testing accuracy of 84.35 percent at an optimal tree depth of 2. Entropy is used as a criteria for splitting.


Metrics of confusion matrix 

accuracy: 0.8435

Precision : 0.5152

Recall or Sensitivity : 0.2429

Specificity : 0.9569

False Positive Rate : 0.0431

False Negative Rate : 0.7571

It can be concluded from the above metrics that our model is not so good in predicting the true positives. It is wrongly predicting actual positives as negative hence the false nagtive rate is as high as 75 %. This is mainly happening due to a huge imbalance in our target where 1233 records are labelled as no and only 237 targets are labelled as yes. To deal with this over sampling and under sampling technique will be applied to dataset and this metrics will be calculated again to check for any improvement in the efficiency of the model.
