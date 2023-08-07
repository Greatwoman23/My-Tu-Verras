# Welcome to My Tu Verras
***

## Task
→ Load the data in a data frame and print the first rows.
→ Make a function that cleans the dataset from lines which any missing values.
→ Plot each attribute in a histogram.
→ Make a function that prints all the histograms.
→ Write a function compute_correlations_matrix to compute Pearson's correlations between every pair of attributes.
→ What is the correlation coefficient between the median value and the number of rooms?
→ Analyse the correlations between the median value and the other attributes. Which attribute is the most negatively correlated with the median value? Does it make sense to you?
→ Plot every attribute against each other.
→ Make a function that prints the scatter matrix.
→ Plot MEDV in function of RM
→ Plot the correlation scatter plot of the median value against LSTAT, AGE, and CRIME.
→ What can you observe? What can you say?.
→ Does the age seems to have any influence on the MEDV?
→ Plot the scatter matrix or print the correlation coefficients for LSTAT. What are the attributes which are the most linearly correlated with LSAT?
→ Make a function that return a New WindowFitted Estimator.
→ Make a second function that will receive the Fitted Estimator and return a prediction.

## Description
The code is using pandas and matplotlib to load, clean, summarize, and visualize a dataset 
about housing prices in Boston. The code defines several functions to perform different tasks, 
such as reading a CSV file, removing missing values, printing histograms, computing correlation 
matrix, and creating scatter matrix. The code also prints some information about the dataset, 
such as its shape, statistical summary, and correlation coefficients. The code aims to explore 
the data and understand how the variables are related to each other and to the target variable. 
This can help in building a predictive model for the housing prices.

## Installation
pip install seaborn scikit-learn

## Usage
The we shared is using two Python libraries: pandas and matplotlib. Pandas is a library for data analysis and manipulation, and matplotlib is a library for data visualization.
The code is divided into several functions, each with a specific purpose:
The load_dataset() function reads a CSV file from a URL and returns a pandas DataFrame object, which is a tabular data structure with rows and columns.
The print_summarize_dataset(dataset) function takes a DataFrame as an argument and prints its dimension, first few rows, and statistical summary (such as mean, standard deviation, min, max, etc.).
The clean_dataset(boston_dataframe) function takes a DataFrame as an argument and removes any rows that have missing values (NaN) using the dropna() method. It returns a cleaned DataFrame.
The print_histograms(boston_dataframe) function takes a DataFrame as an argument and plots a histogram for each column using the plt.hist() function from matplotlib. A histogram is a graphical representation of the distribution of numerical data. It shows how many values fall into each bin or interval.
The compute_correlations_matrix(boston_dataframe) function takes a DataFrame as an argument and computes the correlation matrix using the corr() method. A correlation matrix is a table that shows the correlation coefficients between pairs of variables. A correlation coefficient is a number between -1 and 1 that measures how strongly two variables are related. For example, a correlation coefficient of 0 means no linear relationship, while a correlation coefficient of 1 means a perfect positive linear relationship.
The code also uses the scatter_matrix() function from pandas.plotting to draw a matrix of scatter plots1. A scatter plot is a type of plot that shows the relationship between two variables by plotting them as points on a Cartesian plane. A scatter matrix is a grid of scatter plots that shows the pairwise relationships between multiple variables in a dataset.
This code is using the compute_correlations_matrix(boston_dataframe) function that you defined earlier to calculate the correlation matrix of the boston_data DataFrame. Then, it prints the shape of the correlation matrix, which is a 14 by 14 table, and the correlation coefficients of the ‘MDEV’ column, which is the median value of owner-occupied homes in $1000s. The ‘MDEV’ column is the target variable that we want to predict using the other variables.

The code also defines a new function called print_scatter_matrix(boston_dataframe) that takes a DataFrame as an argument and creates a scatter matrix using the scatter_matrix() function from pandas.plotting. The scatter matrix shows the pairwise relationships between all the variables in the boston_data DataFrame. The function also sets some parameters for the scatter matrix, such as alpha (the transparency of the points), figsize (the size of the figure), diagonal (the type of plot to show on the diagonal), and grid (whether to show grid lines or not). Finally, the function uses the plt.show() function from matplotlib to display the scatter matrix.

The scatter matrix can help you visualize how each variable is related to the others and to the target variable. You can look for patterns, trends, outliers, or clusters in the data. You can also see which variables have strong or weak correlations with each other or with the target variable. This can help you select the most relevant features for your predictive model.



### The Core Team
Oke Temitope Flourish & OluwaKemi Deniran

<span><i>Made at <a href='https://qwasar.io'>Qwasar SV -- Software Engineering School</a></i></span>
<span><img alt='Qwasar SV -- Software Engineering School's Logo' src='https://storage.googleapis.com/qwasar-public/qwasar-logo_50x50.png' width='20px'></span>
