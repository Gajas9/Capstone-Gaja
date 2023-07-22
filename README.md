# Phase 1 Project Template - Minimum Viable Product (MVP)



**Author**: Gaja Sanchayan

## Overview

To provide analysis on car prices in US market to predict what features drives the car prices in US market which will be used by automobile consulting companies to advice potential car Manufacturers.


## Business Problem

To provide analysis on car prices in US market to predict what features drives the car prices in US market which will be used by automobile consulting companies to advice potential car Manufacturers..


## Data
DATA UNDERSTANDING
The analysis is based on a data set of approximately 300 rows and 26 columns on car prices. The data includes many different types of information about each cars. They were categorized in to two different types of data by visualizing using scatter plots
Continuous Data- Wheel base, Car length, curb weight, Engine size, Bore ratio, High mpg etc.
Categorical Data – Car Company, Fuel type, Car body, Drive wheel, Engine location, Engine type, Cylinder number, Fuel system etc.

DATA CLEANING
Categorical Variables
1.Visualization of Categorical data using Box plots 2.Dropping insignificant variables on “Price” of the car 3.Deriving new variable for “Car names” 4.Creating Dummies 
Continuous Variables
1.Visualization of Continuous data and their relation to  Target variable using Heat maps 2. Dropping insignificant variables on “Price” of the car 3. Checking the distribution of Continuous variables using Scatter matrix  and doing Log Transformation


## Modelling

Iteration 1 
Checking for Multi Collinearity and dropped variables which are strongly correlated
Adjusted R square  0.942 but there are many insignificant variables based on the P values
Model Assumptions were checked using modelfit distribution and Regression plots

Iteration 2 
Data was split into Train and test data first to avoid any transformation on test data
Min MAX Scaling on continuous variable and same scaling on test data
Recursive feature elimination to select the important features
 
Adjusted R square  0.917 and all the variables seems to be significant based on the P values except one( engine type)
Dropped the insignificant variable and the and run regression fit
Adjusted R square  0.916 and all the variables seems to be significant


## Model Evaluation

Applied same feature elimination and dropped insignificant variables on the Test data same as train data
Check the Mean Squared Error of both Train and Test data.
There does not seem to be a big difference between the train and test MSE! 
Test MSE is slightly higher than the  training MSE which indicates that the model is performing well on unseen data and is not overfitting to the training data.

## Results

The main features which Contributes heavily on the prices of cars are:
1.Wheelbase
2.Curb weight
3.Horsepower
4.CarCompany_highend brand
5.Enginelocation_rear
6.Carbody_convertible

There is positive relation ship between Price and and these variables.














