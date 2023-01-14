![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

# Predicting Grocery Store Sales - XGBoost

In this project I build a prediction model using gradient boosted trees algorithm (XGBoost Library) to predict sales.

# Results
Features more important to predicting sales are List Price (`Item_MRP`) and how much an item is visible to the consumer in the grocery store (`Item_Visibility`). 

![image](https://github.com/aleivaar94/Grocery-Store-Sales-Prediction/blob/master/images/feature-importance.png)

## Predicting Sales from List Price

![image](https://github.com/aleivaar94/Grocery-Store-Sales-Prediction/blob/master/images/list-price-vs-sales.png)


## Predicting Sales from Item Visibility

![image](https://github.com/aleivaar94/Grocery-Store-Sales-Prediction/blob/master/images/visibility-vs-sales.png)


Train data
𝑅^2 = 0.86
MSE = 390007.2

Test data
𝑅^2 = 0.52
MSE = 1471566.31

# Methodology

## Data Collection

The data was obtained from [Kaggle](https://www.kaggle.com/datasets/brijbhushannanda1979/bigmart-sales-data). The data comes from a grocery store and contains sales data form 2013 for 1559 products across 10 stores in different cities.


## Data Cleaning & Analysis

Two features had more than 15% of missing data. Dropping null values would cause the model to underfit. Instead, missing values are replace with the mean 

`Item_Weight` and `Outlet_Size` have 17% and 28% missing values respectively. By dropping the null values we are loosing an important chunk of data, instead, missing values of `Item_Weight` are replaced with the mean.

`Outlet_Size`, being a categorical variable, is replaced with the mode. After concluding that there is no correlation between among the different `Outlet_Size` options (i.e. High, Medium, Small) and `Outlet_Type`. 

In order to build the prediction model, all features need to have a numerical data type. Therefore, categorical features were encoded into numerical features using LabelEncoder from the sklearn library..

# Conclusion

The model does not predict sales well. A couple of strategies to improve the model are:

- Remove outliers.
- Change the train-test split size.
- Optimize hyperparameters of the gradient boosted trees algorithm.
- Run cross validation
