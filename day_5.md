# Date = 18 June 2024
# PYTHON LIBRARIES
Today i continued with the previous topic and learnt about one more Python Library named Matplotlib.

# Introduction to Matplotlib
Matplotlib is a popular Python library for creating static, interactive and animated visualizations. It provides a flexible and powerful way to generate various types of plots such as line charts, bar charts, histograms, scatter plots and many more. Matplotlib is widely used in data analysis and scientific computing to visualize data in a clear and informative manner. It integrates well with other libraries like NumPy and Pandas making it a go-to tool for plotting and visualizing data. To use it, you typically import it with the command `import matplotlib.pyplot as plt` and then use its functions to create and customize plots.

## What is Matplotlib?
- Matplotlib was created by John D. Hunter.
- Matplotlib is open source and we can use it freely.
- Matplotlib is a low level graph plotting library in python that serves as a visualization utility.
- Matplotlib is mostly written in python, a few segments are written in C, Objective-C and Javascript for Platform compatibility.

## Why We Use Matplotlib?
### Data Visualization: 
Matplotlib provides an easy way to create a wide variety of plots (line, bar, scatter, histograms, etc.) to visualize data patterns, trends, and distributions, making complex data more understandable.
### Customizable Plots:
It allows detailed customization of plots, including colors, labels, legends, titles, axes, and more, making it possible to tailor visualizations to specific needs.
### Integration with Other Libraries:
Matplotlib works seamlessly with libraries like NumPy, Pandas, and Seaborn, enhancing its versatility and enabling efficient data analysis workflows.
### Support for Multiple Plot Types:
Whether you need a simple line plot or complex subplots and 3D visualizations, Matplotlib can handle a wide range of visualization types.
### Wide Adoption and Community Support:
As one of the most widely used Python libraries for plotting, Matplotlib has extensive documentation, a strong community, and numerous tutorials available online, making it easy to learn and troubleshoot.

## What Matplotlib Do ?
### Creates Basic Plots:
It allows you to easily create basic 2D plots like line graphs, scatter plots, bar charts, and histograms to visualize data points and distributions.
### Advanced Plot Customization:
You can fine-tune plot elements like axis scales, tick marks, color schemes, annotations, and grid lines to enhance the clarity of your visualizations.
### Multiple Plotting Options:
You can create multiple plots in one figure (subplots) and organize them in a grid to compare different data sets side by side.
### Interactive Visualization:
Matplotlib supports interactive visualizations, allowing users to zoom in, pan, and save plots in various formats like PNG, SVG, and PDF.
### 3D Plotting: W
With its mplot3d toolkit, Matplotlib also allows for the creation of 3D plots, helping visualize three-dimensional data.


## One Simple Program for plotting a graph using Matplpotlib Library

```python

# importing the required module 
import matplotlib.pyplot as plt 
	
# x axis values 
x = [1,2,3] 
# corresponding y axis values 
y = [2,4,1] 
	
# plotting the points 
plt.plot(x, y) 
	
# naming the x axis 
plt.xlabel('x - axis') 
# naming the y axis 
plt.ylabel('y - axis') 
	
# giving a title to my graph 
plt.title('My first graph!') 
	
# function to show the plot 
plt.show() 


```