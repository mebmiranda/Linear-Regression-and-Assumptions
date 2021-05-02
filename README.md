# Linear-Regression-and-Assumptions

### Objective ###

Generate a linear regression on the advertising dataset and analyze the model. Also, review the regression assumptions and make sure they are met with the model.

The following are the regression assumptions:
  - **Linear Relationship**: There is a linear relationship between the independent variable, x, and the dependent variable, y.
  - **Multicollinearity**: There is no linear relationship between independent variables.
  - **Autocorrelation**: The residuals are independent. In particular, there is no correlation between consecutive residuals in time series data.
  - **Homoscedasticity**: The residuals have constant variance at every level of x.
  - **Residual Normal Distribution** - The residuals of the model should be normally distributed.
 
**Note:** The dataset used in this notebook is the well known 'Advertising Dataset' of ISLR Package.

### Method ### 

 - Observe the relationship between the independent variables and dependent variables using a scatter plot.
 - Generate the Linear Regression Model (Ordinary Least Square).
 - Observe the independence of the residual. Analyze using the Durbin Watson Test.
 - Observe the Homoscedasticity of the model. Analyze by plotting residual vs fitted value .
 - Observe the distribution of the residual. Analyze by plotting the Quartile-Quartile Plot.

### Analysis ##
 - There is a linear relationship between TV and Sales but not between Radio and Sales, and Newspaper and Sales. Hence, Newspaper and Radio are excluded in the regression model.
 - There is no Multicollinearity between the TV, Radio and Newspaper. However, Radio, and Newspaper are still excluded in the model as they do not have a linear relationship with Sales.
 - The Coefficient of Determination is 0.932 which means that 93.2% of the data fit the regression model.
 - The Durbin Watson Test has a value of 1.645 which is within the acceptable range of 1.5 to 2.5. 1.645 means there is a positive low autocorrelation on the residuals.
 - The residual plot shows that there is a Homoscedasticity relationship on the residuals.
 - Quartile - Quartile plot shows that the residuals follow a Normal Distribution.


### Conclusion ###

The generated model has a 93.2% Coefficient of Determination. Only TV is considered as a predictor variable as the other variables do not have a linear relationship with Sales. The generated model passed all the linear regression assumptions.
