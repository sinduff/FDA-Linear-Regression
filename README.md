"# FDA-Linear-Regression" 
Submitted by Sinéad Duffy, ID:10016151
***

### Problem Statement
The goal of this assignment is to accurately predict wind turbine power output from wind speed values using the data contained in the powerproduction dataset.

### 1.0 Introdution
The purpose of this ReadMe file is to provide guidance on navigating the Jupyter Notebook for this module. The notebook was completed to comply with the problem statement outlined above.

The notebook is divided in to a number of different segments namely;

1. Introduction
2. Regression 
3. Regression Explored
4. Conclusion
5. Refrences

The refrences used throughout the notebook are outlined in section 5. Throughout the notebook footnotes are used to indicate where the specific refrences are used.

The notebook also contains a number of cells containing code.  Each of these are outlined in subsequent sections.

### 2.0 Regression
This section looks at regression and provides a definition for it.  The section goes on to look at different types of regression before outlining how regression is used in the real world situtations.


### 3.0 Regression Explored
This section of the notebook looks at different types of regression, and uses the cell codes to explore the differnt types chosen as part of this analysis. 


#### 3.1 Simple Linear Regression
The first type of regression looked at is Simple Linear Regression.  Again, this is defined, with an explanation of each of the variables included.  The section goes on to explore how it is possible to reduce the amount of error on the variables can be completed using the Ordinary Least Squares method.

A section is also included on correlation of the data using Pearson Correlation Coefficient / rsquared value.

The code cells in this section are outlined below;

**Code Cell 1** - this cell code holds the python standard libaries.  The cell must be run first and before any other cell is selected in order for the program to run correctly.

**Code Cell 2** - imports the powerproduction dataframe into the notebook, and then prints the top and tail of it to the screen.

**Code Cell 3** - describes the data that is contained in the dataframe.  Common statistical variables are outlined such as count / mean / standard deviation / min & max values etc.

**Code Cell 4** - this cell depicts the first plot of the notebook.  The plot displays the two variables against each other.  The result displays an 'S' shaped plot.  Some outlier values are displayed at the bottom, where values are zero.  As seen in Cell Code 2, there are zero values contained in the dataset.  The author has made the decision to not remove this outliers as they do contribut to the start of the plot.

**Code Cell 5** - converts the panda's dataframe into a numpy array.  This allows the author to remove each column using *.iloc* into a new array. Printing the *type* of each of the new variables confims that they are now numpy arrays.

**Code Cell 6** - this cell calculates the coefficient of the two variables created in the previous cell.  The coefficient is calcualted using *np.polyfit* and returns values of  **4.91759567** and **-13.89990263** respectively.

**Code Cell 7** - this cell replots the data using the variables from Cell Code 5.  The best fit line is plotted using the coefficient variable calculated in Cell Code 6.  

**Code Cell 8** - this cell outlines the second method of plotting a simple linear regression using numpy and sklearn.   The steps of the analysis has been outlined by from RealPyton and is completed in distinct 5 steps.

**Code Cell 8a** - this cell code outlines the result of the predictive analysis, which is step 5 of method two.  

**Code Cell 9** - this calculates the coefficients / rsquared values for the dataset, as outlined by Pearson's Coefficient Correlation.  The data used are the variables extracted from the dataset in Cell Code 5.

**Code Cell 10** - this plots the correlation for the data set as a whole.

An analysis of the results of the simple linear regression is included, as well as an overview of the two methods employed.


#### 3.2 Polynomial Regression
An overview of the polynomial regression is outlined here, beginning with an explanation of the regression.  A graph outling how by changing the *n*th degree, it is possible to curve the graph to better fit the data.

An explanation of the cell codes used in the analysis are;

**Code Cell 11** - extract x and y variables from the dataframe to allow for analysis using a polynomial regression.  As earlier in the notebook, the new variables are numpy arrays.

**Code Cell 12** the first mapping of the data using a polynomial regression.  The *n*th degree that is used is 1.  The resulting regression line is straight through the data.  The line does interset the data at several points, but is not a good fit for the data set.

**Code Cell 13** uses an *n*th degree of 2.  This curves the regression line slightly, but again, is not representative of the dataset.

**Code Cell 14** uses an *n*th degree of 3.  The regression line does broadly follow the line of the data.  However, the regression line dips well before the data does, so as a method of prediction, there is room for improvement.

An analysis of the results of the polynomial regression is included at the end of the section.  Also included is acknowledgement that this may not be the best method of regression for the dataset.

3.3 Logistic Regression
A brief introduction to logistic regression is included in this section, along with a proposed outline.  The author acknowledges that this may be the best form of regression with which to complete the analysis.

### Conclusion
A brief conclusion of the outcomes of the analysis is included in this section.


### Refrences
The references used throughout the assignment are included here.

