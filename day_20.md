# Date = 09 July 2024
# PROJECT USING PYTHON AND MACHINE LEARNING (DAY 5)
My last week of training will be dedicated to the project work based on my past learning that I have learned during last 15 days of my Training. I am going to develop an project named "Stock Prediction Application" using Python Libraries and Machine Learning Algorithms.
On 5th day of my project I focused on making predictions.

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

# Day 4: Making Predictions

## Objective: 
Use the Trained model to predict stock prices for the next 50 days.

```python 

X = X[:-days]
X_new = X[-days:]  # Use the last 50 rows for predictions

# Make predictions for the next 50 days
prediction = clf.predict(X_new)

# Append the predicted data to the original closing prices
predicted_data = data['close']
final_predictions = np.append(predicted_data, prediction)

# Print the final dataset with predicted future prices
print(final_predictions)

```
---

## Explanation:
1. Predicting Future Prices: I use the last 50 rows of X (the most recent data) to make predictions for the next 50 days using the trained model.
2. Appending Predictions: The predicted stock prices are appended to the original closing prices to create a combined dataset that includes both the historical and predicted future prices.

---

## Tasks Completed:
1. Use the trained model to predict future stock prices (for the next 50 days).
2. Append the predicted prices to the historical data for visualization.

---

## Outcome: 
By the end of Day 5, I have the predicted stock prices for the next 50 days.
