1.  <u>Data Management Commands</u>: These commands are used to manipulate and manage datasets. Some common data management commands in STATA include:

-   ``import:`` reads data into STATA from external sources
-   ``merge:`` combines two or more datasets into a single dataset
-   ``generate``: creates new variables based on existing variables
-   ``replace``: update the value of an existing variable
-   ``egen``: provide access to other library of functions
-   ``drop``: removes variables from a dataset
-   ``keep``: only keeps the specified variables and removes all other
-   ``recode``: changes the values of variables
- ``list``: will list the specific number of rows in the dataset 
	- e.g. ``list in 1/10`` will list the first 10

2.  <u>Descriptive Statistics Commands</u>: These commands are used to compute summary statistics and other measures of central tendency and variability. Some common descriptive statistics commands in STATA include:

-   ``summarize``: computes summary statistics for variables in a dataset
-   ``tabulate``: creates frequency tables for categorical variables
-   ``tabstat``: creates summary statistics for a series of numeric variables
-   ``histogram``: creates a histogram of a continuous variable
-   ``correlation``: computes the correlation between variables

3.  <u>Regression Analysis Commands</u>: These commands are used to perform regression analysis and model relationships between variables. Some common regression analysis commands in STATA include:

-   ``regress``: performs linear regression analysis
-   ``logistic``: performs logistic regression analysis
	- Use ``.or`` to get logistic odds
	![[Pasted image 20230424190517.png]]
	
-   ``probit``: performs probit regression analysis
-   ``robust``: performs robust regression analysis

- ``i`` or ``ib2`` etc: used for categorical variables to specificy which you want as base 
![[Pasted image 20230417165525.png]]
- ``vif``: shows the [[Variance Inflation Factors|VIF]] values (used after the linear regression command)

4.  <u>Graphical Commands</u>: These commands are used to create various types of graphs and plots. Some common graphical commands in STATA include:

-   ``scatter``: creates a scatter plot of two variables
-   ``line``: creates a line plot of one or more variables
-   ``bar``: creates a bar plot of one or more variables
-   ``box``: creates a box plot of one or more variables

5.  <u>Panel Data Commands</u>: These commands are used for analyzing panel data, which is data collected over time for the same individuals or entities. Some common panel data commands in STATA include:

-   ``xtreg``: performs panel data regression analysis
-   ``xtsum``: computes summary statistics for panel data
-   ``xtline``: creates a line plot of panel data

### Logical Operators in STATA
1.  1.  "==" (equal to): This operator returns true if two values are equal.

2.  "!=" (not equal to): This operator returns true if two values are not equal.

3.  ">" (greater than): This operator returns true if the first value is greater than the second value.

4.  ">=" (greater than or equal to): This operator returns true if the first value is greater than or equal to the second value.

5.  "<" (less than): This operator returns true if the first value is less than the second value.

6.  "<=" (less than or equal to): This operator returns true if the first value is less than or equal to the second value.

7.  "&" (and): This operator returns true if both conditions are true.

8.  "|" (or): This operator returns true if at least one of the conditions is true.

9.  "!" (not): This operator reverses the logical result of a condition.
