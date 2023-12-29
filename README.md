# YES-Bank-Stock-Price-Prediction
Yes Bank is a well-known bank in the Indian financial domain. Since 2018, it has been in the news because of the fraud case involving Rana Kapoor. 
Owing to this fact, it was interesting to see how that impacted the stock prices of the company and whether Time series models or any other
 predictive models can do justice to such situations. This dataset has monthly stock prices of the bank since its inception and includes closing, 
starting, highest, and lowest stock prices of every month.

The "Yes Bank Stock Price Prediction" project aims to create a robust machine learning model for forecasting the future price movements of Yes Bank's stock. 
By analyzing historical stock data and relevant financial indicators, the project seeks to provide valuable insights for investors and traders. 
It involves data collection, preprocessing, and feature engineering to create informative input features. 
Various machine learning algorithms will be explored and evaluated to identify the most accurate predictive model. 
Time series analysis techniques will be employed to account for temporal patterns, and sentiment analysis of news and social media will be integrated to capture market sentiment. 
The project's outcome will be a user-friendly interface for real-time predictions, fostering informed decision-making. 
The project's significance lies in its potential to assist stakeholders in navigating the complexities of stock trading by providing reliable forecasts 
and enhancing understanding of key factors influencing Yes Bank's stock prices.

# 1. Solution Strategy

My strategy to solve this challenge was:

Step 01: Know Your Data: Use info(),head(),tail(),find missing values and impute them,remove duplicates.

Step 02: Understand Your Variables: find uniqueness, their datatypes, any irregularity among them,describing variables etc.

Step 03: Data Wrangling & Data Visualization: Explore the data to find insights and better understand the impact of variables on model learning.

Step 04: Machine Learning Modelling: Machine Learning model training.

Step 05: Hyperparameter Fine Tunning: hoose the best values for each of the parameters of the model selected from the previous step.

# 2. Top Data Insights

* Date column is of 'object' datatype we have to convert it to 'datetime'.
* Since we are trying to track variation in stock price on different dates, it makes sense to set this column as index.
* As we can see there are some outliers present in our data. We will need to deal with these before proceeding to modelling.
* We can see that the stock price is rising up until 2018 when the fraud case involving Rana Kapoor happened after which the stock price has had a sharp decline.
* There is a problem of multicollinearity. However since the dataset is so small and has just 3 independent features, multicollinearity is unavoidable here as 
any feature engineering will lead to loss of information.

# 3. Machine Learning Model Applied
At this stage, 4 models were used for analysis:Linear Regression, Lasso Regression, Ridge Regression, Elastic-Net Regression and XGBoost Regression

# 4. Machine Learning Model Performance
## XGBoost Regression:
Mean Absolute Error : 0.0018
Mean squared Error : 0.0424
Root Mean squared Error : 0.0347
R2 score :  0.9899

# 5. Conclusions
1. The popularity of stock closing is growing extremely rapidly day by day which encourage researcher to find new methods if any fraud happens.

2. This technique is used for prediction is not only helpful to researchers to predict future stock closing prices or any fraud happen or not but also helps investors 
or any person who dealing with the stock market in order to prediction of model with good accuracy.

3. In this work we use linear regression technique, lasso regression, ridge regression, elastic net regression and XGBoost Regression technique. T
hese five models gives us the following results

4. High, low, open are directly correlate with the closing price of stocks

5. Target variable(dependent variable) strongly dependent on independent variables

6. Xgboost regression is best model for yes bank stock closing price data this model use for further prediction
