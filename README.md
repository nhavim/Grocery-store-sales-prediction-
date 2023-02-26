Regression Project (Time Series) Sales Prediction for a Grocery Store.
0 Introduction
This project is a time series forecasting problem. We will predict store sales on data from Corporation Favorita, a large Ecuadorian-based grocery retailer.
The aim is to predict sales for each product family and store combinations. There are 6 datasets given (Train, Test, Store, Transactions
Holidays and Events, and Daily Oil Prices).

1.2. Problem statement
We are to build a Machine Learning model that will accurately predict the unit sales for thousands of items sold at different Favorita stores.

1.3 Data Handle
First of all, different libraries were imported for processing the data. The different data sets were loaded from CSV files. Each data set was inspected using pandas commands like the head(), tail(), info(), shape, dtype(), and unique().

2.0 Questions and Hypotheses

This section dealt with questioning and hypothesis formulation based on the information gathered from exploring the data. Two sets of hypotheses were formulated, and 10 questions were asked to further help in exploring the data.

2.1 Hypotheses
a. Null Hypothesis (H0): Change in oil price has no significant change in total sales.

Alternative Hypothesis (H1): Changing oil prices significantly affects total sales.

b. Null Hypothesis (H0): Promotion does not positively affect total sales.

Alternative Hypothesis (H1): Promotion positively affects total sales.

2.2 Questions
I. Is the training dataset complete (has all the required dates)?

II. Which dates have the lowest and highest sales for each year?

III. Did the earthquake impact sales?

IV. Are certain groups of stores selling more products? (Cluster, city, state, type)

V. Are sales affected by promotions, oil prices, and holidays?

VI. What analysis can we get from the date and its extractable features?

VII. What is the difference between RMSLE, RMSE, and MSE (or why is the MAE greater than all of them?)

VIII. What are the daily sales of each store?

IX. Do the dates for paying public sectors affect sales?

X. What is the trend in sales?

3.0 Feature processing:

Here is the section to clean and process the features of the dataset.

3.1 Ensuring quality data.
Different libraries including Pandas, Numpy, Seaborn, and matplotlib were installed to help us process the data. The data sets were loaded and inspected. Elements that were wrongly placed were moved to their rightful columns. Each column in the different data sets was called and inspected to ensure the quality of the data. The different data sets were merged using pd.merge() function to form a wholistic data frame.

4.0 Answering the questions.
Data visualization was carried out to better understand the data.

4.1 Is the training dataset complete (has all the required dates)?
Analyzing the data revealed that 25 December of each year was missing. It could be either because of the Christmas festivity or the stores do not open during Christmas.

4.2 Question 2. Which dates have the lowest and highest sales for each year?


Right from 2013, the first week of January every year recorded a downward trend in sales. Sales increase gradually to the middle of the year and decline again but by December record the highest sales across the years. Thus, from 2013 to 2017. Undoubtedly sale in 2017 was generally high compared to the previous years. Specifically, on February 9, 2013, sales across all stores were 416.1763K which was the lowest sales ever recorded by the grocery store likewise on April 1, 2017, the total sales across the store were 1.463084M recording the highest sales in the history of the grocery store.

4.3 Did the Earthquake impact sales?


From the graph above, two weeks before the Earthquake struck Ecuador (2016–04–01 to 2016–04–13), sales were generally low. But two weeks after the Earthquake (2016–04–17 to 2016–04–29), general sales increased. This could be a result of panic buying. An increase in sales could also be attributed to a festive occasion such as Easter which is celebrated around that same period of the year.

4.4 Are certain groups of stores selling more products? (Cluster, city, state, type)





From the four graphs (Cluster, city, state, type) above, certain groups of stores sell more products than others.

4.5 Are sales affected by promotions, oil prices, and holidays?


Promotion, Oil prices and holidays have all influenced sales.

4.6 What analysis can we get from the date and its extractable features?




The three graphs are time series graphs which display the yearly, month and daily trends in sales for from 2013 to 2017.

4.7 What is the difference between RMSLE, RMSE, and MSE (or why is the MAE greater than all of them?)

MAE (Mean Absolute Error) is the sum of absolute differences between actual and predicted values. It doesn’t consider the direction, that is positive or negative.

MSE (Mean Squared Error) is always positive and a value closer to 0 or lower value is better.

RMSE (Root Mean Square Error) is obtained by taking the square root of the mean squared error.

Root Mean Square Log Error (RMSLE) is the root mean square error calculated on the logarithmic scale.

4.8 What are the daily sales of each store?


4.9 From the graph, payday has an effect on sales. It can be observed that sales go up at the middle and end of each month and payment of the public servants is every two weeks falls on every 15 and the end of every month.


4.10 Question 10. What is the trend in sales over the years?

5.0 Conclusion and Recommendation
The final part talks about the over findings and recommendations for future decision-making.

This has not reached its concluding part. The final part will be published in a few days to come. Thank you
