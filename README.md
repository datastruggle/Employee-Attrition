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
