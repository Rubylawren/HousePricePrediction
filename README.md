# HousePricePrediction
## Overview
This project focuses on predicting house prices using the Boston Housing dataset available on Kaggle. The primary task involved in this project include data cleaning, handling missing values, detecting and dealing with outliers, and building a predictive model. 

## Table of Contents

1. [Project Description](#project-description)
2. [Dataset](#dataset)
3. [Data Preprocessing](#data-preprocessing)
    - [Handling Missing Values](#handling-missing-values)
    - [Detecting and Handling Outliers](#detecting-and-handling-outliers)
4. [Model Building](#model-building)
5. [Results](#results)
6. [How to Use](#how-to-use)
7. [Dependencies](#dependencies)
8. [Conclusion](#conclusion)

## Project Description

The goal of this project is to predict the prices of houses based on various features available in the Boston Housing dataset. The project involves several steps:
- Data cleaning to ensure quality data for the model
- Handling missing values
- Detecting and handling outliers using z-scores
- Building and evaluating a predictive model

## Dataset

The dataset used in this project is the Boston Housing dataset from Kaggle, which includes features such as:
- CRIM: per capita crime rate by town
- ZN: proportion of residential land zoned for lots over 25,000 sq. ft.
- INDUS: proportion of non-retail business acres per town
- CHAS: Charles River dummy variable (= 1 if tract bounds river; 0 otherwise)
- NOX: nitric oxides concentration (parts per 10 million)
- RM: average number of rooms per dwelling
- AGE: proportion of owner-occupied units built prior to 1940
- DIS: weighted distances to five Boston employment centers
- RAD: index of accessibility to radial highways
- TAX: full-value property tax rate per $10,000
- PTRATIO: pupil-teacher ratio by town
- B: 1000(Bk - 0.63)^2 where Bk is the proportion of Black residents by town
- LSTAT: % lower status of the population
- MEDV: Median value of owner-occupied homes in $1000s (target variable)

## Data Preprocessing

### Handling Missing Values

Missing values in the dataset can lead to inaccurate predictions and model inefficiencies. In this project, missing values are handled as follows:
- For numerical features, missing values are filled with the mean value of the respective feature.
- There were no categorical features in the dataset.

### Detecting and Handling Outliers

Outliers can skew the data and affect the performance of the predictive model. We use the z-score method to detect and handle outliers:
- Calculate the z-score for each data point in numerical features.
- Define a threshold (e.g., z-score > 3 and z-score < -3) to identify outliers.
- Remove data points that are identified as outliers based on the z-score threshold.

## Model Building

After preprocessing the data, several machine learning models were built and evaluated. These models include:
- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor

The models are evaluated using R-squared score.

## Results

The best-performing model is selected based on the evaluation metrics. 
