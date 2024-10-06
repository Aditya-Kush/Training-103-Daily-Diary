# Date = 03 July 2024
# PROJECT USING PYTHON AND MACHINE LEARNING (DAY 1)
- My last week of training will be dedicated to the project work based on my past learning that I have learned during last 15 days of my Training. I am going to develop an project named "Stock Prediction Application" using Python Libraries and Machine Learning Algorithms.
- On 1st day of my project I focused on Installing required libraries for the project, setting up API Key and Definition of Problem Scope.

---

## Project Overview

### Objective:
The goal of this project is to predict the future stock prices using historical data. I will use Linear Regression, A basic Supervised learning algorithm to build a model that can predict stock prices for the next 50 days based on historical prices from the past.

### Python Libraries Used:

1. numpy: For array manipulation.
2. pandas_datareader: For fetching financial data from Alpha Vantage.
3. matplotlib: For visualizing stock price data and predictions.
4. sklearn: For machine learning preprocessing, splitting, and building the linear regression model.
5. datetime: To handle date operations.


### Machine Learning Algorithm:
Linear Regression: A linear regression model is used to predict future stock prices based on historical features (open, high, low, close, volume).

---

# Day 1: Project Setup and Data Fetching

## Goal:
1. I Set up the project environment, Installed  necessary libraries(Pandas and datetime) and fetch the historical stock data using the Alpha Vantage API.
2. Ensure we can access the stock market data for Apple Inc. (AAPL) from the given start date (January 1, 2010) to the current date.

---

```python

# Importing necessary libraries
import pandas_datareader as pdr
import datetime as dt

# Define stock symbol and time range
stock_symbol = 'AAPL' 
start_date = dt.datetime(2010, 1, 1)
end_date = dt.datetime.now()

# Fetch historical stock data from Alpha Vantage
data = pdr.data.DataReader(stock_symbol, 'av-daily', start=start_date, end=end_date, api_key='YOUR_ALPHA_VANTAGE_API_KEY')

# Print first few rows of the data to check
print(data.head())

```
---

## Explanation of the Above written Code:
1. pandas_datareader: It is a library that allows fetching stock market data from various sources including Alpha Vantage. In this project, I used the "av-daily" endpoint which provides daily historical data.

2. datetime: It is used to define the time period for which I fetched the stock data. I set the start_date as January 1, 2010, and the end_date as the current date (dt.datetime.now()).

3. After fetching the data, I printed the first few rows (data.head()) to verify that the data was pulled correctly.

---


## Task Completed:
### 1. Installed Required Libraries:
Ensured I have all the necessary libraries installed via pip (e.g. pandas_datareader, sklearn, matplotlib, etc.).

### 2. Set up API Key:
- Registered with Alpha Vantage and received my free API key.
- Integrated the API key into the script for fetching historical stock data.

### 3. Defined Problem Scope:
- Stock price prediction for Apple (AAPL) using historical data from 2010 to the present.
- The stock data includes features like open, high, low, close, and volume.

---

## Outcome:
I successfully fetched the stock data for Apple Inc. (AAPL) from January 1, 2010, to the current date. The dataset included key fields such as open, high, low, close, and volume which are essential for financial analysis.