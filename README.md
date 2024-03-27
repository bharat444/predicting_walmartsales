# Problem Statement 
Conventional retail stores still play a prominent role in a world dominated by Ecommerce. Retail is the process of selling consumer goods or services to customers through multiple channels of distribution to earn a profit. From groceries to clothing to electronics, customers keep flooding the gates of retail stores to satisfy their needs. As time has passed, retailers have had to evolve in order to keep up with changes in demands and the ever-changing mindset of customers. One such retail industry juggernaut that has kept up with the demands of customers as well changed the face of the retail industry for the better is Walmart Inc.

Walmart Inc is an American multinational retail corporation that operates a chain of hypermarkets, discount department stores, and grocery stores, headquartered in Bentonville, Arkansas. They have many stores across the globe and it is the largest retail company by revenue.

## Dataset

The dataset used is the [Walmart Sales Prediction](https://www.kaggle.com/divyajeetthakur/walmart-sales-prediction) from Kaggle.

We are given historical sale s data for 45 Walmart stores located in different regions. Each store contains a number of departments. Apart from these, weekly data of Fuel price, Holiday, Temperature with some other features are also present in the data set.

In addition, Walmart runs several promotional markdown events throughout the year. These markdowns precede prominent holidays, the four largest of which are the Super Bowl, Labour Day, Thanksgiving, and Christmas. The weeks including these holidays are weighted five times higher in the evaluation than non-holiday weeks.

Data consists of 421570 records of weekly sales from stores spanning between ’05-Feb-2010’ to ’26-Oct-2012’. This comprises of 143 Weeks of sales data.

Total 16 numbers of attributes are provided in the Data set including Target variable. Attribute definition is:

**Target Variable: Weekly Sales**
<br>
**Store:** The store number
<br>
**Size:** Size of the Store
<br>
**Dept:** Department of the Store
<br>
**Date:** Specifying the Week (Friday of every Week)
<br>
**Temperature:** Average temperature in the region (in ℉)
<br>
**FuelPrice:** Cost of fuel in the region
<br>
**CPI:** Consumer price index
<br>
**Unemployment:** Unemployment rate
<br>
**IsHoliday:** Whether the week is a special holiday week


## Models Used

1. Linear Regression: This model is most useful in data which is linearly correlated. It simply finds the "Best fit coefficients" by using the standard linear regression formula.

2. Support Vector Machine: This model is also very useful when the data is linearly correlated. Although, SVMs are capable of projecting the data into greater dimensions to find out better patterns.

3. Decision Tree Classifier: This model identifies the most informative attribute at every level and uses it to make a tree. The final tree can then be used as a simple if-else statement to identify the final prediction.

## Future Work
1. We can perform Hyperparameter Tuning on the models used to find out how much the accuracy can be improved.
2. We can try using Neural Networks.
3. We can try to get more data and make time-based features to create time-dependent or sequence-dependent models.
