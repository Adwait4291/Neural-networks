# Plotting a Quadratic Function

This repository contains a simple Python script using NumPy, Matplotlib, and Seaborn to plot a quadratic function (y = x^2).

## Description

The script generates a set of x values using `np.linspace` within a specified range (-100 to 100 in this case). It then calculates the corresponding y values using the equation y = x^2. Finally, it plots the function using Matplotlib, with Seaborn providing a visually appealing style.

## Code

```python
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
sns.set()

x = np.linspace(-100, 100, 1000)

print(x)

len(x)

plt.plot(x) # Plots x vs index, not the quadratic

y = np.square(x)

y

plt.plot(x, np.square(x)) # Plots the quadratic function

plt.plot(x, y) #Redundant, same as above

plt.plot(x, y, c='r') # Plots the quadratic in red
plt.xlabel("x") # Adding label for x axis
plt.ylabel("y = x^2") # Adding label for y axis
plt.title("Plot of y = x^2") # Adding title to the plot
plt.grid(True) # Adding grid lines
plt.show() # To display the plot

##Dependencies

NumPy
Matplotlib
Seaborn

You can install these libraries using pip:

pip install numpy matplotlib seaborn

##Output

The script will generate a plot of the quadratic function y = x^2, with the x-axis ranging from -100 to 100. The plot will be displayed in red, as specified in the code.  The x and y axis will be labelled along with a title. Grid lines will also be displayed to improve readability.


## Explanation of the Code

Import Libraries: Imports NumPy for numerical operations, Matplotlib for plotting, and Seaborn for styling.
Generate x values: Creates an array of 1000 evenly spaced x values between -100 and 100 using np.linspace.
Calculate y values: Calculates the square of each x value and stores it in the y array.
Plot the function: Uses plt.plot(x, y, c='r') to plot y against x, with the line color set to red.
Labels and Title: Adds labels to the x and y axes using plt.xlabel and plt.ylabel, and a title to the plot using plt.title.
Grid Lines: Adds grid lines to the plot for better readability using plt.grid(True).
Show the plot: Displays the generated plot using plt.show().
