# Used Car Price price analysis and price prediction
An analysis of used vehicle dataset containing 426880 samples to understand the various features and their correlations on the vehicle price. 

## Contents
- Summary
- Objective
- Data Understanding
- Data Preparation
- Modeling
- Evaluation
- Recommendations 


## Summary
Used vehicle sales have generally increased over the past 40 years. However, there have been some notable downturns, such as the recession of 2008-2009 and the COVID-19 pandemic in 2020. There are a number of factors that contribute to the demand for used vehicles. One is the cost of new vehicles have become increasingly expensive in recent years, making them out of reach for many consumers. Used vehicles offer a more affordable option for people who need a reliable vehicle.A nother factor that drives demand for used vehicles is the increasing reliability of used cars as they are now more reliable than ever before. This means that consumers can feel confident buying a used car without having to worry about it breaking down.

## Objective
Analyze the used vehicle dataset to understand the various factors that make a vehicle more or less expensive. Develop a price prediction model using three regression models - Linear, Ridge(GridSearchCV) and Lasso to predict vehicle price. Analyze the impact of core features like odometer, age, type, manufacturer, condition, drive type to examine the relationships and to understand the factors that decides the price.

## Data Understanding
Used vehicle dataset from Kaggle is used for analysis. Dataset contained 426,880 samples and after analyzing for missing, duplicate and non critical features, sample size is reduced to 97078. On analyzing what the data can tell, vehicles older than 1980, priced less than 1000 and more than 125k is been purged from the dataset. Outliers are removed to avoid overfitting or underfitting issues. 

## Data Preparation
Non numerical features are preprocessed using scikit-learn labelencoder, scaled and transformed to a degree of 2. GridSearchCV with 5-fold cross validation for analyzing hyperparameters.

## Modeling
Scikit-learn regression models - linear, ridge and Lasso models develop to identify the best model for price prediction.

## Evaluation
![Screenshot](model_comparison.png)

## Recommendations
