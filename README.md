In this project, the team is comparing traditional time series methods with regression models for sales forecasting at Walmart Inc. Using the Walmart Dataset from Kaggle, the team assesses the accuracy of each method and selects the best-performing model to predict future sales accurately.

# Abstract:
This project investigates the efficacy of traditional time series methods versus regression models for sales forecasting in the retail sector, focusing on Walmart Inc. Utilizing the Walmart Dataset from Kaggle, various predictive algorithms including Auto Regressor (AR), Moving Average (MA), Auto-Regressive Integrated Moving Average (ARIMA), Seasonal ARIMA (SARIMA), Holt-Winters’ Method (HW), Decision Tree, Random Forest, and XGBoost are compared based on metrics like Mean Absolute Error (MAE), Mean Square Error (MSE), and Root Mean Square Error (RMSE). The project aims to identify the most accurate model to optimize resource allocation and profit maximization strategies for Walmart Inc.

About Dataset
Walmart Inc. is an American multinational retail corporation that operates a chain of hypermarkets (also called supercenters), discount department stores, and grocery stores in the United States, headquartered in Bentonville, Arkansas. The company was founded by Sam Walton in nearby Rogers, Arkansas in 1962 and incorporated under Delaware General Corporation Law on October 31, 1969. It also owns and operates Sam's Club retail warehouses. In India, Walmart operates under the name of Flipkart Wholesale.
 **Source** : The dataset utilized in this research was sourced from the well-known dataset site Kaggle (https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting). The data's dependability is increased by Kaggle's trustworthiness as a source. The Walmart is the source of this dataset. In a recruiting competition, job-seekers project sales for 45 Walmart stores and select holiday markdown events. This competition showcases modelling mettle and counts towards rankings and achievements.

**Dataset**: Walmart has provided historical weekly sales data from 45 stores from 2010 to 2012, totalling 421,570 instances. Each store has around 90 departments. The dataset includes five CSV files: Features, Stores, Train, Test, and SampleSubmission, which will be used for Project submission.

<img src="https://github.com/kandelsatish/Walmart_Sales_Prediction/blob/main/static/images/hello_walmart.jpg" alt="alt text" width="1900" height="400">

# How does Walmart use Big Data?
Improving Store Checkout: By using Predictive Analysis, the stores can anticipate demand at a certain week and determine how many Sales Representatives / Employees are needed.
Managing the Steps of Supply Chain: The company optimizes the routes to the shipping dock and tracks the number of times the product is accessed before it reaches the Customer's destination. Also, it uses the data to analyze transportation lanes and routes for the company's trucks. These data help Walmart keep transportation costs down and schedule an appropriate time for drivers.
Optimizing Product Assortment: By analyzing customer preferences and shopping patterns, Walmart accelerates the decision-making on how to maintain stocks. Big Data provides insights on new items and discontinued products.
Personalizing Shopping Experience: With Big Data, Walmart analyzes the shopping preferences of the customers to develop a consistent and delightful shopping experience.
and much more…

# Features Description:
**Store**: This column represents the store number or identifier. It is numerical and each number corresponds to a specific store.

**Date**: Indicates the date of data collection or event, formatted as a month.

**Weekly_Sales**: A numerical value representing the total sales achieved in a week. The values are in decimal format, allowing for precise measurement of sales.

**Holiday_Flag**: This binary flag indicates whether the given date was a holiday (1) or not (0).

**Temperature**: Represents the temperature on that specific day, it’s in decimal format which allows for an accurate representation of the temperature.

**Fuel_Price**: Indicates the price of fuel on that particular day, represented as a decimal number to provide precise values.

**CPI**: Stands for Consumer Price Index, a measure that examines the average change over time in consumer prices for goods and services. It’s also represented as a decimal number.

**Unemployment**: This column shows unemployment rates, represented as decimals to provide detailed information.

# 

# Observation:
- Time series models outperform regression models, especially Holt-Winters (HW), due to their ability to predict past values.
  
- Regression models may not capture complex patterns in time series data due to reliance on known attributes.
  
- Limited correlation between attributes and weekly sales may have hindered regression model performance.
  
- Improvement areas include increasing hyperparameter tuning parameters, applying Holt-Winters to all stores and departments, and addressing technical issues with WMAE.



