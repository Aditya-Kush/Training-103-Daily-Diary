# Date = 13 June 2024
# PYTHON LIBRARIES
Today i learnt about one of the python Library named Numpy.

# Python Libraries
Python’s standard library is very extensive offering a wide range of facilities as indicated by the long table of contents listed below. The library contains built-in modules (written in C) that provide access to system functionality such as file I/O that would otherwise be inaccessible to Python programmers as well as modules written in Python that provide standardized solutions for many problems that occur in everyday programming. A Python library is a collection of pre-written code, functions, and modules that you can use to perform common tasks without having to write the code from scratch. These libraries help save time and effort by providing ready-made solutions for a wide range of programming problems. 
Python has a vast ecosystem of libraries for tasks such as data analysis (e.g., NumPy, Pandas), Machine learning (e.g., TensorFlow, scikit-learn) and more. To use a library in Python, you typically install it via pip (Python's package manager) and import it into your project.

# Introduction to NumPy

## What is NumPy?
- NumPy was created in 2005 by Travis Oliphant. It is an open source project and you can use it freely.
- NumPy stands for Numerical Python.
- NumPy is a Python library used for working with arrays.
- It also has functions for working in domain of linear algebra, fourier transform, and matrices.

## Why Use NumPy?
- In Python we have lists that serve the purpose of arrays but they are slow to process Therefore NumPy aims to provide an array object that is up to 50x faster than traditional Python lists.
- The array object in NumPy is called ndarray and it provides a lot of supporting functions that make working with ndarray very easy.
- Arrays are very frequently used in data science, where speed and resources are very important.

## One Simple Program for Creating a NumPy Array

```python

import numpy as np
arr = np.array([1, 2, 3, 4, 5])
print(arr)
print(type(arr))

```