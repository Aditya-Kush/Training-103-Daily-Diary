# Date = 05 July 2024
# PROJECT USING PYTHON AND MACHINE LEARNING (DAY 3)
My last week of training will be dedicated to the project work based on my past learning that I have learned during last 15 days of my Training. I am going to develop an project named "Stock Prediction Application" using Python Libraries and Machine Learning Algorithms.
On 3rd day of my project I focused on Feature Engineering, Scaling and Data Preparation.

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

# Day 3: Feature Engineering and Scaling

## Goal:
1. Prepare the feature set (X) and target variable (Y) for training the machine learning model.
2. Scale the features to ensure they are normalized and improve the performance of the model.

--- 

```python

import numpy as np
from sklearn import preprocessing

# Prepare feature variables (X) and target variable (Y)
X = np.array(data.drop(['shift'], axis=1))  # All columns except 'shift'
Y = np.array(data['shift'])  # 'shift' column as the target

# Scale the features using StandardScaler
X = preprocessing.scale(X)

# Print first few rows of features and target
print(X[:5], Y[:5])

```
---

## Explanation:
1. I separated the feature variables (X) and the target variable (Y). X consists of all columns except for the shift column (which contains the future price) and Y is the shift column itself.

2. Scaling: I applied the StandardScaler to scale the feature variables to ensure that they are on the same scale. Standardizing the features (mean = 0, variance = 1) is important because it helps the model converge faster and improves its accuracy. This is especially relevant for linear regression models.

--- 

## Task Completed:
### 1. Feature Engineering:
- Dropped the 'shift' column from the features (X), as it was only the target variable (Y).
- Converted the data to NumPy arrays for easier matrix manipulations.

### 2. Scaling the Features:
- Used StandardScaler from sklearn.preprocessing to scale the data (features like open, high, low, close, volume) to a standard range (mean=0, variance=1). 
- This helps the linear regression model perform better as it is sensitive to the magnitude of features.

### 3. Data Preparation:
- Split the data into X (features) and Y (target) for training and testing.
- Split the data into training and test sets (80% training, 20% testing) using train_test_split from sklearn.model_selection.

---

## Outcome:
The feature set was successfully prepared and scaled. Scaling is crucial to ensure the model performs optimally, especially with linear regression.