# Date = 04 July 2024
# PROJECT USING PYTHON AND MACHINE LEARNING (DAY 2)
My last week of training will be dedicated to the project work based on my past learning that I have learned during last 15 days of my Training. I am going to develop an project named "Stock Prediction Application" using Python Libraries and Machine Learning Algorithms.
- On 2nd day of my Project I focused on shifting of values and Missing Values

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

# Day 2: Data Preprocessing - Shift Column and Missing Values

## Goal:
- I Created a column called shift that holds the closing prices shifted by 50 days,which will act as the target variable (i.e. future stock prices).
- It can Handle any missing values that result from the shift operation.

---

``` python

# Define the number of days to predict (future prediction window)
days = 50

# Create a 'shift' column to store the closing price shifted by 50 days (target for prediction)
data['shift'] = data['close'].shift(-days)

# Drop missing values (NaN) resulting from the shift operation
data.dropna(inplace=True)

# Print the updated data
print(data.head())

```
---

## Explanation:
1. The shift(-days) function shifts the closing prices by 50 days. This means that for each day in the dataset, the corresponding shift column will contain the closing price 50 days ahead. This column will act as the target variable (Y) in our prediction model.
2. I removed the rows that contained missing values (NaN) which arise due to the shift operation. Since the last 50 rows will not have a future price to predict, they are dropped using dropna().

---

## Outcome:
The data was successfully prepared with the shift column representing future prices (50 days ahead) and the missing values were handled appropriately.
