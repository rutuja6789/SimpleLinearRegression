# SimpleLinearRegression
This is an example of simple linear regression using height-weight dataset.

Some important parameters that should be considered are the 
1) R-squared value, 
2) Adj. R-squared value, 
3) F-statistic, prob(F-statistic), 
4) coef of intercept and input variables, 
5) p>|t|.

R-Squared is the coefficient of determination. A statistical measure that says much percentage of data points are falling on the best fit line. An R-squared value closer to 1 is expected for a model to fit well.

Adj. R-squared penalizes the R-squared value if we keep adding the new features which are not contributing to the model prediction. If Adj. R-squared value < R-squared value, it’s a sign that we have irrelevant predictors in the model.

F-statistic or F-test helps us to accept or reject Null Hypothesis. It compares the intercept-only model with our model with features. The null hypothesis is ‘all of the regression coefficients are equal to zero and that means both the models are equal’. The alternate hypothesis is ‘intercept the only model is worse than our model, which means our added coefficients improved the model performance.

If prob(F-statistic) < 0.05 and F-statistic being a high value, we reject the Null hypothesis. It signifies that there is a good relationship between the input and the output variables.

coef shows the estimated coefficients of the corresponding input features

T-test talks about the relation between the output and each of the input variables individually. The null hypothesis is ‘coef of an input feature is 0’. The alternate hypothesis is ‘coef of an input feature is not 0’.

If pvalue < 0.05, we reject the null hypothesis which indicates that there is a good relationship between the input variable and the output variable. We can eliminate the variables whose pvalue is >0.05.

In this case, the R-squared value (0.855) is close to Adj. R-squared value (0.855) is a good sign that the input features are contributing to the predictor model.

F-statistic is a high number and p(F-statistic) is almost 0, which means our model is better than the only intercept model.

pvalue of t-test for input variable is less than 0.05, so there is a good relationship between the input and the output variable.
