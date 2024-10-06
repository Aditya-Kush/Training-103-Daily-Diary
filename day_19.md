# Date = 08 July 2024
# PROJECT USING PYTHON AND MACHINE LEARNING (DAY 4)
My last week of training will be dedicated to the project work based on my past learning that I have learned during last 15 days of my Training. I am going to develop an project named "Stock Prediction Application" using Python Libraries and Machine Learning Algorithms.
On 4th day of my project I focused on Train-Test Split and Model Training.

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

# Day 4: Train-Test Split and Model Training

## Goal:
1. Split the data into training and test sets (80% for training and 20% for testing).
2. Train a linear regression model and evaluate its accuracy.

```python

from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression

# Split the data into training (80%) and testing (20%) sets
X_train, X_test, Y_train, Y_test = train_test_split(X, Y, test_size=0.2)

# Initialize and train the linear regression model
clf = LinearRegression()
clf.fit(X_train, Y_train)

# Evaluate the model on the test data
accuracy = clf.score(X_test, Y_test)
print(f"Model Accuracy (R^2 Score): {accuracy}")

``` 
---

## Explanation:
1. train_test_split: This function splits the data into training and test sets. 80% of the data is used for training while 20% is used for testing.
2. I trained the Linear Regression model using the fit() function on the training data (X_train and Y_train).
3. I evaluated the model’s accuracy using the R² score on the test set (X_test and Y_test). The R² score indicates how well the model explains the variance in the target variable (future stock prices).

---

## Task Completed:
### 1. Model Training:
Used LinearRegression from sklearn.linear_model to train the model on the training data (X_train, Y_train).

### 2. Model Evaluation:
Evaluated the accuracy of the model using the test data (X_test, Y_test) by calculating the coefficient of determination (R² score) which indicates how well the model fits the test data. Printed the accuracy score of the model.

---

## Outcome:
The linear regression model was trained and tested and I obtained an R² score that indicates how well the model is predicting future stock prices. The model is performing reasonably well but there is always room for improvement which will be addressed in later stages.


