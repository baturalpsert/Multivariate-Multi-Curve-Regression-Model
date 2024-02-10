# Multivariate Multi-Curve Regression Model
Welcome to my Multivariate Multi Curve Regression study! In this study, first of all, a multivariate multi-curve regression model is created using the Pyomo library in Python. The purpose of the study is to observe how accurate results can be obtained by creating an original prediction model by making the normally univariate multi-curve regression model multivariate with the help of Pyomo and integrating cosine similarity, and by predicting the oil prices for the coming months.

Our data is for training 2020/01 - 2022/10, for testing 2022/10 - 2023/6. Here K represents the number of curves, M represents the polynomial degree. Models can be created to include K and M {1,2,3}, but here K = 3, M = 1 model is used as an example. After the model is created, the objective function and polynomial formulas are calculated. Graphs are created to observe better. Then, all of the training data is separated into 65% training and 35% test to use to test how well cosine similarity does assignment. The main purpose of using cosine similarity is to assign the test data to the curve with the highest cosine similarity score by comparing each test data with all of the training data. After testing, cosine similarity study is done between the real test data and the real training data and the curve of the training data with the highest cosine similarity score is assigned to the test data. Oil price prediction value is calculated on this curve.
