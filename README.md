# Final Project

*Thanh Tung Ha Thuc*
*Ironhack Data Analytics - March 2021 cohort*

## Walmart Recruiting - Store Sales Forecasting

## Content

- Project Description (Introduction)
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
2. Analyze and predict Weekly Sales using a machine learning model, in this case I chose Simple Linear Regression and Multiple linear Regression.

## Dataset

The data is from Kaggle and was provided by Walmart. It containts historical sales data for 45 Walmart stores located in different regions. 
Each store contains a number of departments.

### Table descriptions

**stores.csv**

Contains anonymized information about the 45 stores, indicating the type and size of store.

**train.csv**

The historical training data, which covers to 2010-02-05 to 2012-11-01. Within this file we will find the following fields:

- Store - the store number
- Dept - the department number
- Date - the week
- Weekly_Sales -  sales for the given department in the given store
- IsHoliday - whether the week is a special holiday week

**test.csv**

This file is identical to train.csv, except we have withheld the weekly sales.

**features.csv**

This file contains additional data related to the store, department, and regional activity for the given dates. It contains the following fields:

- Store - the store number
- Date - the week
- Temperature - average temperature in the region
- Fuel_Price - cost of fuel in the region
- MarkDown1-5 - anonymized data related to promotional markdowns that Walmart is running. MarkDown data is only available after Nov 2011, and is not available for all stores all the time. Any missing value is marked with an NA.
- CPI - the consumer price index
- Unemployment - the unemployment rate
- IsHoliday - whether the week is a special holiday week
