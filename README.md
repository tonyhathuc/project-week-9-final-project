# Final Project

*Thanh Tung Ha Thuc*
*Ironhack Data Analytics - March 2021 cohort*

## Kaggle Competition - Walmart Sales Forecasting
<img src="./images/Walmart.jpg"/>

## Content

- Project Description 
- Dataset
- Stack
- Project management
- In this repository
- Conclusions
- Challenges
- Extra Steps



## Project Description

This project is to be submitted to Ironhack to prove that the student is capable of executing a project from beginning to end 
in one week.

For my final project I chose a Kaggle Competition, where the aim was to:
  - Analyze what impact Weekly Sales
  - Predict Weekly Sales using Machine Learning models such as Multiple Linear Regression (as our baseline model) and KNeighboursRegressor, Decision Tree Regressor and Random Forest Regressor.


## Dataset

The data is from [kaggle](https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting/data) provided by Walmart and contains historical sales data for 45 Walmart stores located in different regions. Each store contains a number of departments. 

If you wish to learn more about the table descriptions, they can be found [here](https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting/data).

## Stack
Python
 - numPy and Pandas for data cleaning and wrangling
 - Seaborn, MatPlotLib and Plotly for data visualisations
 - SciKitLearn for Machine Learning Deployment
 - Google Slides for presentation

## Project Management
- Trello
- Notion

## In this repository:

- In the [code](https://github.com/tonyhathuc/project-week-9-final-project/tree/master/code) folder, you can find the jupyter notebook with python code used to access, clean and train the data for our machine learning models.
- In the [data](https://github.com/tonyhathuc/project-week-9-final-project/tree/master/data) folder you can find the .csv files that contains the data that have been worked with.

## Conclusions
- Holiday seasons contributes to spike in Weekly Sales
- In terms of sales, 2012 was the weakest in sales compared to 2010, 2011
- Most features have no linear relationship with Weekly Sales.
- There is correlation between Year and Fuel Price, which makes sense as fuel prices change every year.
- The R2 score of our baseline model (Multiple Linear Regression) was just 0.9 and the difference between the actual and predicted value is high, which makes the model not fit for prediction.
- Random Forest Regressor performed the best, with the accuracy of 95.93%, second was Decision Tree Regressor with 94.93% followed by KNeighboursRegressor with 34.99%. 
- Random ForestRegressor wins as it generally produces better results and work well on large dataset and is able to work with missing data by creating estimates for them.

## Challenges
- Large dataset
- Time constraint
- Basically no correlation with the target variable

## Extra Steps
- More Feature Engineering
- Use LogisticRegression to research how much do Holiday Seasons impact Weekly Sales.
