# Date = 14 June 2024
# PYTHON LIBRARIES
Today i continued with the previous topic and learnt about one more Python Library named Pandas.

# Introduction to Pandas
Pandas is an open-source library that is built on top of NumPy library. It is a Python package that offers various data structures and operations for manipulating numerical data and time series. It is mainly popular for importing and analyzing data much easier. Pandas is fast and it has high-performance & productivity for users.
Pandas is a powerful and open-source Python library. The Pandas library is used for data manipulation and analysis. Pandas consist of data structures and functions to perform efficient operations on data.

## What is Pandas?
•⁠  ⁠The name "Pandas" has a reference to both "Panel Data" and "Python Data Analysis" and was created by Wes McKinney in 2008.
- Pandas is a powerful and versatile library that simplifies the tasks of data manipulation in Python. Pandas is well-suited for working with tabular data, such as spreadsheets or SQL tables.
- The Pandas library is an essential tool for data analysts, scientists and engineers working with structured data in Python.
•⁠  ⁠Pandas is a Python library used for working with data sets.
•⁠  ⁠It has functions for analyzing, cleaning, exploring and manipulating data.

## Why Use Pandas?
•⁠  ⁠Relevant data is very important in data science.
•⁠  ⁠Pandas allows us to analyze big data and make conclusions based on statistical theories.
•⁠  ⁠Pandas can clean messy data sets and make them readable and relevant.

## What Can Pandas Do?
Here is a list of things that we can do using Pandas.
- Data set cleaning, merging and joining.
- Easy handling of missing data (represented as NaN) in floating point as well as non-floating point data.
- Columns can be inserted and deleted from DataFrame and higher-dimensional objects.
- Powerful group by functionality for performing split-apply-combine operations on data sets.
Data Visualization.
⁠- Pandas are also able to delete rows that are not relevant or contains wrong values like empty or NULL values. This is called cleaning the data.
•⁠  ⁠Pandas gives you answers about the data. 
 ⁠Like:
1.  ⁠Is there a correlation between two or more columns?
2.  ⁠What is average value?
3.⁠  ⁠Max value?
4.⁠  ⁠Min value?

##Installing Pandas
The first step in working with Pandas is to ensure whether it is installed in the system or not.  If not, then we need to install it on our system using the pip command.

## Follow these steps to install Pandas:

### Step 1: 
Type ‘cmd’ in the search box and open it.
### Step 2:
Locate the folder using the cd command where the python-pip file has been installed.

### Step 3:
After locating it, type the command 'pip install pandas'.

## Importing Pandas
After the Pandas have been installed in the system, you need to import the library. This module is generally imported by command 'import pandas as pd'

## One Simple Program for Creating a series using Pandas Library

```python

import pandas as pd 
import numpy as np

# Creating empty series 
ser = pd.Series() 
print("Pandas Series: ", ser) 

# simple array 
data = np.array(['g', 'e', 'e', 'k', 's']) 
  
ser = pd.Series(data) 
print("Pandas Series:\n", ser)

```

