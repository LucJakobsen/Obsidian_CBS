- ``NumPy`` = used in almost all numerical computation in Python.  
- ``Pandas`` = used for data manipulation and analysis, in particular data structures and operations for manipulating numerical tables and time series
- ``Matplotlib`` = graphics library for generating scientific figures
- ``Seaborn`` = built on top of Matplotlib and offers sane choices for plot style and color defaults, defines simple high-level functions for common statistical plot types, and integrates with the functionality provided by Pandas
	- Seaborn is more user-friendly


### NumPy
``import numpy as np``

***NumPy functions and uses:***
[[NumPy Examples]]
- ``np._version_`` = will check the installed version of NumPy
- ``np.array([])`` = will create an array
- ``np.linspace()`` = returns a range of evenly spaced numbers


### Pandas
``import pandas as pd``

***Pandas functions and uses:***
[[Pandas Examples]]


### Matplotlib
``import matplotlib.pyplot as plt``
``%matplotlib inline``
The inline ensures that the graphs are displayed in the notebook instead of a pop-out window

***Matplotlib functions and uses:***
[[Matplotlib Examples]]
- ``plt.figure()`` = will create a new figure or activate and existing figure
- ``plt.plot()`` = will plot y versus x as lines and/or markers
- ``plt.xlabel()`` = will set/name the x axis
- ``plt.ylabel()`` = will set/name the y axis
- ``plt.title()`` = will add a title to the graph
- ``plt.show()`` = will show/display all open figures
- ``plt.subsplots()`` = creates a figure and a set of subplots
- ``plt.hist()`` = will plot a histogram
- ``plt.scatter()`` = will plot a scatterplot
- ``plt.pie()`` = will plot a pie chart
- ``plt.step()`` = will create a step chart
- ``plt.bar()`` = will create a bar chart
- 

- ``fig.savefig()`` = will save a figure in the chosen format (e.g. ``savefig("figure.png")``)
- 



### Seaborn
``import seaborn as sn``

***Seaborn functions and uses:***
[[Seaborn Examples]]
- ``sns.set_style`` = will set the style of the graph
- ``sns.kdeplot`` = will create a kernel density estimation (smoother histogram basically)
- ``sns.pairplot`` = will visualize he multidimensional relationships among variables
- ``sns.FacetGrid`` = used to visualize the distribution of a variable or the relationship between multiple variables separately within subsets
	- Basically it creates a grid which you can insert graphs into
- ``sns.catplot`` = will create a categorical plot (used for plotting categorical variables)
- ``sns.jointplot`` = shows the joint distribution between  different datasets
