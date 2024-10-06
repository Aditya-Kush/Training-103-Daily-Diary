# Date = 10 July 2024
# PROJECT USING PYTHON AND MACHINE LEARNING (DAY 6)
My last week of training will be dedicated to the project work based on my past learning that I have learned during last 15 days of my Training. I am going to develop an project named "Stock Prediction Application" using Python Libraries and Machine Learning Algorithms.
On 6th day of my project I focused on Visualization and Result Analysis.

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

# Day 6: Visualization and Results Analysis

## Objective: 
Visualize both the historical stock prices and the predicted future prices.

---

```python

# Drop rows with missing values (NaN) if any
data.dropna(inplace=True)

# Plot the original stock prices and the predicted stock prices
plt.figure(figsize=(10,5))
plt.plot(data['close'], 'r', label='Original Prices')  # Original prices in red
plt.plot(np.arange(len(data), len(data) + days), prediction, linewidth=0.5, label='Predicted Prices')  # Predicted prices
plt.title(f'{stock_symbol} Stock Price Prediction')
plt.xlabel('Date')
plt.ylabel('Price')
plt.legend(title="Stock Price Prediction")
plt.show()

```

---

## Explanation:
1. Plotting: I used matplotlib to plot both the original stock prices and the predicted future prices. The red line represents the historical stock prices and the predicted future prices are shown in blue.
2. Visualization: This visualization helps to compare the actual vs predicted stock prices and assess the model's performance visually.

---

## Tasks Completed:
1. Visualize the original stock prices and the predicted future stock prices using matplotlib.
2. Analyze the results visually.

---

## Outcome:
By the end of Day 6, I am having a visual comparison of the historical stock prices and the predicted future prices.

---

## 6 Days Learning Summary of this Project
1. In this project, I set out to predict the future stock prices of Apple Inc. (AAPL) using Linear Regression, A machine learning technique. Over the course of the project, I first collected historical stock data from Alpha Vantage using the pandas_datareader library. The data spanned from January 1, 2010, to the current date and included daily stock prices like open, high, low, close and volume. To create a target for prediction, I shifted the closing prices by 50 days enabling the model to forecast the stock's future value.

2. After cleaning the data and scaling the features using standardization, I split the data into training and test sets then trained the Linear Regression model and evaluated its accuracy using the R² score which showed how well the model could explain the variance in the stock prices. With the model trained, I predicted stock prices for the next 50 days and combined these predictions with the original historical data to visualize the results.

3. The predictions were plotted alongside the actual stock prices allowing for a visual comparison. While the model showed some promise, It was clear that Linear Regression might not capture the complex, non-linear patterns typically seen in stock prices which are influenced by a multitude of factors. In conclusion, this project provided valuable insights into stock price forecasting using machine learning and it has motivated me to explore more advanced models like LSTM or Random Forest in the future for potentially better accuracy.



