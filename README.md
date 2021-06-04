# Final Project

*Thanh Tung Ha Thuc*
*Ironhack Data Analytics - March 2021 cohort*

## Walmart Recruiting - Store Sales Forecasting

## Content

- Project Description 
- Objective
- Dataset
- Stack
- Conclusion
- Challenges
- Future analysis
- Project management


## Project Description

This project is to be submitted to Ironhack to prove that the student is capable of executing a project from beginning to end 
in one week.

I chose a kaggle competition for my final project as I wanted to go through the experience of participating on a challenge that 
counts towards ranking and achievements.

## Objective

1. Analyze what impacts Weekly Sales.
2. Analyze and predict Weekly Sales using Simple Linear Regression and Multiple linear Regression.

## Dataset

The data is from [kaggle](https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting/data) provided by Walmart and contains historical sales data for 45 Walmart stores located in different regions. 
Each store contains a number of departments.

### Table descriptions

#### stores.csv

Contains anonymized information about the 45 stores, indicating the type and size of store.

**train.csv**

The historical training data, which covers to 2010-02-05 to 2012-11-01. Within this file we will find the following fields:

- Store - the store number
- Dept - the department number
- Date - the week
- Weekly_Sales -  sales for the given department in the given store
- IsHoliday - whether the week is a special holiday week

#### test.csv

This file is identical to train.csv, except we have withheld the weekly sales.

#### features.csv

This file contains additional data related to the store, department, and regional activity for the given dates. It contains the following fields:

- Store - the store number
- Date - the week
- Temperature - average temperature in the region
- Fuel_Price - cost of fuel in the region
- MarkDown1-5 - anonymized data related to promotional markdowns that Walmart is running. MarkDown data is only available after Nov 2011, and is not available for all stores all the time. Any missing value is marked with an NA.
- CPI - the consumer price index
- Unemployment - the unemployment rate
- IsHoliday - whether the week is a special holiday week

## Stack
- With Python
..*numPy and Pandas for cleaning and wrangling
..*Seaborn, MatPlotLib and Plotly for visualisations
..*SciKitLearn for machine learning deployment
..*Google Slides for presentation

## Project Management
- Trello

## In this repository:

- In the folder code you can find the jupyter notebook with python code used to access the data, clean it and train our machinel earning model.
- Data folder contains the .csv files 

## Conclusions
- Holiday seasons contributes to spike in Weekly Sales
- In terms of sales, 2012 was the weakest in sales compared to 2010, 2011
- Most features have no linear relationship with Weekly Sales.
- There is correlation between Year and Fuel Price, which makes sense.
- The r2 score of our Multiple Linear Regression model was just 0.069 and the difference between the actual and predicted value is high. 
- Thus Multiple Linear Regression is not the right model for this prediction.
- For this challenge, other models such as DecisionTreeRegressor, GradientBoostingRegressor or RandomForestRegressor generally produce better results as they work well on large datasets, and are able towork with missing data by creating estimates for them.

## Limitation
- Large dataset
- Time constraint
- Basically no correlation with the target variable

## Extra Steps
- More Feature Engineering
- Try DecisionTreeRegressor and RandomForestRegressor
- Use LogisticRegression to see how much do holiday seasons impact Weekly Sales
