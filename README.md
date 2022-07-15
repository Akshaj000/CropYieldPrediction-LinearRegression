# CropYieldPrediction-LinearRegression


Crop yield prediction is one of the challenging tasks in agriculture. It plays an essential role in decision making at global, regional, and field levels. This is part of our maths project to understand linear regression models.  
  
We have removed categories and id parameter from the dataframe. This is because category contained multiple categories which was complicated to represent as numbers. We handled Nan value for each column by replacing it with the median of that column. We had to replace one of the uv value which crossed 5000 which effected the data representation.
  
The prediction of crop yield here is based on water, fertiliser_usage, pesticides, area, uv and region parameters. We have used Linear regression to create various models with combination of various such parameters. We calculated root mean square error for each model and found the best model with least rmse. We are also checking r square value to get the score of each model.  
  
we selected this dataset https://www.kaggle.com/datasets/jaahnavigundapu/crop-yield-prediction-using-machine-learning . Unfortunately this only gave us score upto 0.68 using Linear Regression and upto 90 using polynomial regression.

## Terms and concepts that are used

[Linear Regression](https://www.ibm.com/in-en/topics/linear-regression#:~:text=Resources-,What%20is%20linear%20regression%3F,is%20called%20the%20independent%20variable.)
 
Linear regression analysis is used to predict the value of a variable based on the value of another variable. The variable you want to predict is called the dependent variable. The variable you are using to predict the other variable's value is called the independent variable.

[Polynomial Regression](https://www.javatpoint.com/machine-learning-polynomial-regression)

Polynomial Regression is a regression algorithm that models the relationship between a dependent(y) and independent variable(x) as nth degree polynomial.

[Pandas](https://www.kaggle.com/learn/pandas)

pandas is a fast, powerful, flexible and easy to use open source data analysis and manipulation tool,
built on top of the Python programming language.
  
[Numpy](https://numpy.org/)

NumPy brings the computational power of languages like C and Fortran to Python, a language much easier to learn and use. With this power comes simplicity: a solution in NumPy is often clear and elegant.

[Matplotlib](https://matplotlib.org/)

Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python. Matplotlib makes easy things easy and hard things possible.

[Seaborn](https://seaborn.pydata.org/)

Seaborn is a Python data visualization library based on matplotlib. It provides a high-level interface for drawing attractive and informative statistical graphics.

[Scikit-learn](https://scikit-learn.org/stable/)

Scikit-learn (Sklearn) is the most useful and robust library for machine learning in Python. It provides a selection of efficient tools for machine learning and statistical modeling including classification, regression, clustering and dimensionality reduction via a consistence interface in Python. This library, which is largely written in Python, is built upon NumPy, SciPy and Matplotlib.

[Statsmodels](https://www.statsmodels.org/stable/index.html)

statsmodels is a Python module that provides classes and functions for the estimation of many different statistical models, as well as for conducting statistical tests, and statistical data exploration. An extensive list of result statistics are available for each estimator. The results are tested against existing statistical packages to ensure that they are correct.

[Data analysis](https://en.wikipedia.org/wiki/Data_analysis)

Data analysis is a process of inspecting, cleansing, transforming, and modelling data with the goal of discovering useful information, informing conclusions, and supporting decision-making.Data analysis has multiple facets and approaches, encompassing diverse techniques under a variety of names, and is used in different business, science, and social science domains. In today's business world, data analysis plays a role in making decisions more scientific and helping businesses operate more effectively.

[Data visualisation](https://www.ibm.com/cloud/learn/data-visualization#:~:text=Data%20visualization%20is%20the%20representation,that%20is%20easy%20to%20understand.)

Data visualization is the representation of data through use of common graphics, such as charts, plots, infographics, and even animations. These visual displays of information communicate complex data relationships and data-driven insights in a way that is easy to understand.

[Heatmap](https://pythonbasics.org/seaborn-heatmap/)

A heat map is a plot of rectangular data as a color-encoded matrix. As parameter it takes a 2D dataset. That dataset can be coerced into an ndarray.

This is a great way to visualize data, because it can show the relation between variables including time.

[Histplot](https://seaborn.pydata.org/generated/seaborn.histplot.html)

Histograms are visualization tools that represent the distribution of a set of continuous data. In a histogram, the data is divided into a set of intervals or bins (usually on the x-axis) and the count of data points that fall into each bin corresponding to the height of the bar above that bin. These bins may or may not be equal in width but are adjacent (with no gaps).  

[Jointplot](https://seaborn.pydata.org/generated/seaborn.jointplot.html)

A Jointplot comprises three plots. Out of the three, one plot displays a bivariate graph which shows how the dependent variable(Y) varies with the independent variable(X). Another plot is placed horizontally at the top of the bivariate graph and it shows the distribution of the independent variable(X).


[Regplot](https://seaborn.pydata.org/generated/seaborn.regplot.html)

This method is used to plot data and a linear regression model fit.

[Training and Testing data](https://www.obviously.ai/post/the-difference-between-training-data-vs-test-data-in-machine-learning)

Train/Test is a method to measure the accuracy of your model.
It is called Train/Test because you split the the data set into two sets: a training set and a testing set. You train the model using the training set. You test the model using the testing set.

[Mean squared error](https://www.statisticshowto.com/probability-and-statistics/statistics-definitions/mean-squared-error/)

![](https://www.gstatic.com/education/formulas2/443397389/en/mean_squared_error.svg)

The mean squared error (MSE) tells you how close a regression line is to a set of points. It does this by taking the distances from the points to the regression line (these distances are the “errors”) and squaring them. The squaring is necessary to remove any negative signs. It also gives more weight to larger differences. It’s called the mean squared error as you’re finding the average of a set of errors. The lower the MSE, the better the forecast.

[Root mean squared error](https://www.statisticshowto.com/probability-and-statistics/regression-analysis/rmse-root-mean-square-error/)

![](https://www.gstatic.com/education/formulas2/443397389/en/root_mean_square_deviation.svg)

Root Mean Square Error (RMSE) is the standard deviation of the residuals (prediction errors). Residuals are a measure of how far from the regression line data points are; RMSE is a measure of how spread out these residuals are. In other words, it tells you how concentrated the data is around the line of best fit. Root mean square error is commonly used in climatology, forecasting, and regression analysis to verify experimental results.

[R square value](https://statisticsbyjim.com/regression/interpret-r-squared-regression/)

![](https://www.gstatic.com/education/formulas2/443397389/en/coefficient_of_determination.svg)


R^2	=	coefficient of determination  
RSS	=	sum of squares of residuals  
TSS	=	total sum of squares   

R-squared (R2) is a statistical measure that represents the proportion of the variance for a dependent variable that's explained by an independent variable or variables in a regression model. Whereas correlation explains the strength of the relationship between an independent and dependent variable, R-squared explains to what extent the variance of one variable explains the variance of the second variable. So, if the R2 of a model is 0.50, then approximately half of the observed variation can be explained by the model's inputs.

[Correlation](https://www.statisticshowto.com/probability-and-statistics/correlation-analysis/)


Correlation is used to test relationships between quantitative variables or categorical variables. In other words, it’s a measure of how things are related. 

[Covariance](https://corporatefinanceinstitute.com/resources/knowledge/finance/covariance/#:~:text=In%20mathematics%20and%20statistics%2C%20covariance,the%20variance%20between%20two%20variables.)

![](https://www.gstatic.com/education/formulas2/443397389/en/covariance_formula.svg)


cov_x,y	=	covariance between variable x and y  
x_i	=	data value of x  
y_i	=	data value of y  
!bar_x	=	mean of x  
!bar_y	=	mean of y  
N	=	number of data values  

In mathematics and statistics, covariance is a measure of the relationship between two random variables. The metric evaluates how much – to what extent – the variables change together. In other words, it is essentially a measure of the variance between two variables. However, the metric does not assess the dependency between variables.

#### Here is more about ML models in agriculture

- [Link 1](https://www.google.com/search?q=AI+and+ML+in+agriculture&oq=AI+in+agriculture&aqs=chrome..69i57.4425j0j4&sourceid=chrome&ie=UTF-8) 
- [Link 2](https://github.com/Akshaj000/NaiveBayesClassifier_CropRecommender)

#### Feel free to correct my work and send a PR. Would love to hear more about Regression models and their use in Agriculture and other sector.



