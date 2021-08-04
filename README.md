# Project_PR
The purpose of this project is to classify a person into most appropriate health
category based on their physical attributes, daily activities, food habits, etc...
using Machine Learning techniques.

Data Pre-Processing:
The given Datatset consists of combination of Numerical and Categorical Data.
Support Vector machines built with sci-kit learn doesn’t natively support Categorical Data.

In order to use categorical data with sci-kit learn Support Vector Machines,we have to do One-hot Encoding.
One-hot Encoding helps in converting columns with categorical data intmultiple columns of binary values.

get_dummies from pandas does the One-hot encoding for us.

Once the data pre processing is done, we can classify and observe the performance of various ML models(Here SVM and KNN), through certain metrics(accuracy).

Feature selection:
To reduce the computations and try to improve the accuracy, we do the process of feature selection to train our model with only selected number of features which has 
major contribution towards predicting the class.

A single feature selection method cannot be applied to our dataset since we have a combination of both continuous(numerical) and categorical data.

So, we separate our Categorical and Numerical data,then apply PCA(Principal Component Analysis) to our Numerical data
and Pearson’s Chi-Squared method of feature selection to our Categorical data.
 
 
