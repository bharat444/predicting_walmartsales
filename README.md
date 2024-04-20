In this project, the team is comparing traditional time series methods with regression models for sales forecasting at Walmart Inc. Using the Walmart Dataset from Kaggle, the team assesses the accuracy of each method and selects the best-performing model to predict future sales accurately.

# Abstract:
This project investigates the efficacy of traditional time series methods versus regression models for sales forecasting in the retail sector, focusing on Walmart Inc. Utilizing the Walmart Dataset from Kaggle, various predictive algorithms including Auto Regressor (AR), Moving Average (MA), Auto-Regressive Integrated Moving Average (ARIMA), Seasonal ARIMA (SARIMA), Holt-Winters’ Method (HW), Decision Tree, Random Forest, and XGBoost are compared based on metrics like Mean Absolute Error (MAE), Mean Square Error (MSE), and Root Mean Square Error (RMSE). The project aims to identify the most accurate model to optimize resource allocation and profit maximization strategies for Walmart Inc.

# About Dataset
Walmart Inc. is an American multinational retail corporation that operates a chain of hypermarkets (also called supercenters), discount department stores, and grocery stores in the United States, headquartered in Bentonville, Arkansas. The company was founded by Sam Walton in nearby Rogers, Arkansas in 1962 and incorporated under Delaware General Corporation Law on October 31, 1969. It also owns and operates Sam's Club retail warehouses. In India, Walmart operates under the name of Flipkart Wholesale.

**Source**: The dataset utilized in this research was sourced from the well-known dataset site Kaggle (https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting). The data's dependability is increased by Kaggle's trustworthiness as a source. The Walmart is the source of this dataset. In a recruiting competition, job-seekers project sales for 45 Walmart stores and select holiday markdown events. This competition showcases modelling mettle and counts towards rankings and achievements.

**Dataset**: Walmart has provided historical weekly sales data from 45 stores from 2010 to 2012, totalling 421,570 instances. Each store has around 90 departments. The dataset includes five CSV files: Features, Stores, Train, Test, and SampleSubmission, which will be used for Project submission.

<img src="https://github.com/kandelsatish/Walmart_Sales_Prediction/blob/main/static/images/hello_walmart.jpg" alt="alt text" width="1900" height="400">

# How does Walmart use Big Data?
Improving Store Checkout: By using Predictive Analysis, the stores can anticipate demand at a certain week and determine how many Sales Representatives / Employees are needed. Managing the Steps of Supply Chain: The company optimizes the routes to the shipping dock and tracks the number of times the product is accessed before it reaches the Customer's destination. Also, it uses the data to analyze transportation lanes and routes for the company's trucks. These data help Walmart keep transportation costs down and schedule an appropriate time for drivers. Optimizing Product Assortment: By analyzing customer preferences and shopping patterns, Walmart accelerates the decision-making on how to maintain stocks. Big Data provides insights on new items and discontinued products. Personalizing Shopping Experience: With Big Data, Walmart analyzes the shopping preferences of the customers to develop a consistent and delightful shopping experience. and much more…

# Parameters Selected:

**Store**: This is the store number, and it ranges from 1-45
**Dept**: It is the department number, it ranged from 1-99, for different categories of items.
**Date**: The Week
**IsHoliday**: whether that specific week has a special holiday in it
**Weekly_Sales**: Store weekly total amount in USD
**Temperature**: The average weekly temperature of the particular store region in Fahrenheit
**Fuel_Price**: Cost of Fuel of the particular store region in USD
**MarkDown1-5**: Anonymized Data related to Walmart's promotional markdown is only available after November 2011, and not all stores have it
**CPI**: Consumer Price Index of specific store region for the week
**Unemployment**: The unemployment rate of a particular store region for the month
**Type**: Type of the store, A, B or C
**Size**: Size of the specific store measured in square feet
# 

# Observation:
- Time series models outperform regression models, especially Holt-Winters (HW), due to their ability to predict past values.
  
- Regression models may not capture complex patterns in time series data due to reliance on known attributes.
  
- Limited correlation between attributes and weekly sales may have hindered regression model performance.
  
- Improvement areas include increasing hyperparameter tuning parameters, applying Holt-Winters to all stores and departments, and addressing technical issues with WMAE.



