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

# Methodologies Applied

![image](https://github.com/bharat444/predicting_walmartsales/assets/110676765/d481b89e-b4d6-4439-b01c-ac875efbf1af)

# Time Series and Regression method comparison

<img width="668" alt="Screenshot 2024-04-19 at 9 20 22 PM" src="https://github.com/bharat444/predicting_walmartsales/assets/110676765/a6780ea7-13fa-468b-8365-670657f5b850">

The models are compared against each other using performance measures of MSE, MAE, RMSE. HW has the lowest error in MAE, MSE, and RMSE, and it is the best model to predict the test set from the train set. Surprisingly, the time series models perform much better than regression models.

# Observation:

- Time series models outperform regression models, especially Holt-Winters (HW), due to their ability to predict past values.
  
- Regression models may not capture complex patterns in time series data due to reliance on known attributes.
  
- Limited correlation between attributes and weekly sales may have hindered regression model performance.
  
- Improvement areas include increasing hyperparameter tuning parameters, applying Holt-Winters to all stores and departments, and addressing technical issues with WMAE.

# Challenges:

- **Data quality**: Ensuring the quality and completeness of the Walmart Dataset from Kaggle, including handling missing values, outliers, and inconsistencies.
  
- **Complex relationships**: Capturing and modelling the complex relationships between various factors influencing sales, such as seasonality, promotions, economic conditions, and consumer behaviour.

- **Model selection**: Choosing the most appropriate predictive algorithms from a wide range of options, considering factors like interpretability, scalability, and computational complexity.
  
- **Overfitting**: Preventing overfitting of the models to the training data, especially in regression models with a high number of features, to ensure generalizability to unseen data.
  
- **Scalability**: Ensuring that the selected models can scale effectively to handle the large volume of data from Walmart's thousands of stores worldwide.
  
- **Interpretability**: Balancing the need for accurate predictions with the requirement for interpretable models that stakeholders can understand and trust in making management decisions.
  
- **Deployment**: Overcoming challenges related to deploying the selected model into production, including integration with existing systems, maintenance, and monitoring.
  
- **Resource constraints**: Managing resource constraints, such as computing power, time, and expertise, throughout the project lifecycle, especially given the scale and complexity of the Walmart retail environment.
  
# Future Scope:

- **Expansion to other retail sectors**: Extend the project's scope to other retail sectors beyond Walmart, exploring how similar predictive models can be applied to different industries such as fashion, electronics, or automotive.

- **Real-time sales forecasting**: Develop real-time sales forecasting capabilities to enable Walmart and other retailers to react promptly to changing market conditions and consumer behaviour, leveraging streaming data and advanced analytics.
  
- **Incorporation of external data sources**: Integrate additional external data sources, such as weather data, social media trends, or economic indicators, to enhance the accuracy and granularity of sales predictions.
  
- **Personalized marketing strategies**: Use predictive analytics to tailor marketing strategies and promotions to individual customer preferences, optimizing customer engagement and loyalty.
  
- **Inventory optimization**: Extend the project to include inventory optimization capabilities, leveraging predictive analytics to forecast demand more accurately and optimize inventory levels across Walmart's extensive supply chain network.
  
- **Expansion to omnichannel retailing**: Adapt the predictive models to support omnichannel retailing, encompassing both online and offline sales channels, to provide a seamless shopping experience for customers and optimize overall sales performance.
  
- **Collaboration with suppliers**: Collaborate with Walmart's suppliers to share sales forecasts and demand predictions, fostering better coordination and efficiency in the supply chain.
  
- **Integration with IoT and sensor data**: Explore the integration of Internet of Things (IoT) devices and sensor data from stores and warehouses to capture real-time insights into customer behavior, product popularity, and inventory movement.
  
- **Predictive analytics for pricing optimization**: Extend the project to include pricing optimization capabilities, using predictive analytics to determine optimal pricing strategies for different products and market segments, maximizing revenue and profitability.

# Used Libraries and Modules

1. **numpy (np)**: NumPy is used for numerical computing and provides support for large, multi-dimensional arrays and matrices, along with a collection of mathematical functions.

2. **pandas (pd)**: Pandas are used for data manipulation and analysis, providing data structures and operations for manipulating numerical tables and time series data.

3. **flask**: Flask is a micro web framework for building web applications in Python. It is used in this project to create a web interface for users to input movie names and receive recommendations.

4. **sklearn**: Scikit-learn is a machine learning library in Python, that provides simple and efficient tools for data mining and data analysis. In this project, it is used for feature extraction, model training, and evaluation.

5. **CountVectorizer**: CountVectorizer is a feature extraction technique used for converting text data into numerical feature vectors. It is commonly used in natural language processing tasks, such as sentiment analysis.

6. **cosine_similarity**: Cosine similarity is a measure of similarity between two vectors by measuring the cosine of the angle between them. It is used in this project to compute the similarity between movie descriptions for recommendation purposes.

7. **json**: The JSON module provides functions for encoding and decoding JSON data. It is used for parsing JSON responses from APIs.

8. **bs4 (Beautiful Soup)**: Beautiful Soup is a Python library for web scraping. It is used in this project to scrape user reviews from the IMDb website.

9. **urllib.request**: The urllib.request module is used for opening and reading URLs. It is used in conjunction with Beautiful Soup for web scraping.

10. **pickle**: The pickle module is used for serializing and deserializing Python objects. It is used in this project to save and load machine learning models.

11. **requests**: The requests module is used for making HTTP requests in Python. It is used to fetch movie details and posters from the TMDb API.

12. **tmdbv3api (TMDb)**: TMDb is a Python wrapper for The Movie Database (TMDb) API. It is used in this project to fetch movie details and posters for recommendation purposes.

# Used Tools and Technologies

- GitHub
  
- GitLab
  
- Google Collaborator
  
- Canva
  
- Zoom & Teams


# References:

- Bonnes, K. (2014). Predictive analytics for supply chains: A systematic literature review. In 21st Twente Student Conference on IT. Netherlands.

- Catal, C., Kaan, E. C. E., Arslan, B., & Akbulut, A. (2019). Benchmarking of regression algorithms and time series analysis techniques for sales forecasting. Balkan Journal of Electrical and Computer Engineering, 7(1), 20-26.

- Hüülsmann, M., Borscheid, D., Friedrich, C. M., & Reith, D. (2012). General sales forecast models for automobile markets and their analysis. Trans. MLDM, 5(2), 65-86.

- Jain, A., Menon, M. N., & Chandra, S. (2015). Sales forecasting for retail chains.

- Knott, B., Liu, H., & Simpson, A. (2015). Predicting sales for Rossmann drug stores.

- Lasek, A., Cercone, N., & Saunders, J. (2016). Restaurant sales and customer demand forecasting: Literature survey and categorization of methods. In Smart City 360° (pp. 479-491). Springer, Cham.

- Makatjane, K. D., & Moroke, N. D. (2016). Comparative study of Holt-Winters triple exponential smoothing and seasonal ARIMA: Forecasting short term seasonal car sales in South Africa. Risk Governance and Control: Financial Markets and Institutions, 6(1), 71-82.

- Massaro, A., Maritati, V., & Galiano, A. (2018). Data mining model performance of sales predictive algorithms based on RapidMiner workflows. International Journal of Computer Science & Information Technology (IJCSIT), 10(3), 39-56.

- Mentzer, J. T., & Moon, M. A. (2004). Sales forecasting management: A demand management approach. Sage Publications.


