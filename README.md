# Multiple-Regression-Problem- Building multiple regression model using SAS

Problem: A national chain of women’s clothing stores with locations in the large shopping malls
thinks that it can do a better job of planning more renovations and expansions if it
understands what variables impact sales. It plans a small pilot study on stores in 25
different mall locations. The data it collects consist of monthly sales, store size (sq. ft),
number of linear feet of window display, number of competitors located in mall, size of
the mall (sq. ft), and distance to nearest competitor (ft).
1. Define a multiple regression model for the data. 
2. Interpret the values of the coefficients in the model. 
3. Test whether the model as a whole is significant. At the 0.05 level of significance,
what is your conclusion? 
4. Use the model to predict monthly sales for each of the stores in the study. 
5. Find and interpret the value of �2 for this model. 
6. Test the individual regression coefficients (i.e., check the result of test statistics
that SAS or Excel provides). At the 0.05 level of significance, what are your
conclusions? 
7. If you were going to drop just one variable from the model, which one would you
choose? Why?

Solution: 
1.	Multiple Regression Model
Y = B0 + B1X1 + B2X2
<img width="264" alt="image" src="https://user-images.githubusercontent.com/63497057/204067115-d17f6d34-fd0d-489d-a990-287824764f70.png">
<img width="340" alt="image" src="https://user-images.githubusercontent.com/63497057/204067121-a76b46a8-2d21-4857-9808-bb4dfe02b26a.png">
<img width="340" alt="image" src="https://user-images.githubusercontent.com/63497057/204067127-d63d489c-0965-4e03-96dc-53203bc81c47.png">

2.

<img width="341" alt="image" src="https://user-images.githubusercontent.com/63497057/204067145-6b1e17c2-853f-44fa-96d3-3d19706af4b1.png">

  a.	The intercept(β0) in regression table tells us the average expected value for the response variable when all of the predictor variables are equal to zero. In this example, the regression coefficient for the intercept is equal to 1506.80179.

  b.	The regression coefficient for size is 0.91937.

  c.	The regression coefficient for window is 9.07598

  d.	The regression coefficient for a number of Competitors is 67.68553

  e.	The regression coefficient for Mall Size is -0.00090285	

  f.	The regression coefficient for Nearest Competitor is 2.09589

3.	First, we get table for Analysis of Variance which shows f statistics to determine the significance of model. At α = 0.05, this regression is significant because p-value is less than 0.05. 
4.	We can use the parameter estimate values in this table to predict monthly sales for each of the stores in the study.
Monthly sales = 1506.80179+ 0.91937*(size) + 67.68553*(No. Competitor) -0.0009(Mall Size) 
1506.80179+ 0.91937*(3580) + 67.68553*(18) -0.0009(685900)
5.	Coefficient of determination(r2) shows that about 83% variation in Sales is explained by the Regression. We get not big difference between R-Square and Adjusted R Square because we have only 5 independent variables, if data had more independent variables the difference would have been larger. It also says that it is a good model.
6.	The t-test result in Parameter Estimate tables shows all independent variables are showing significant estimates, except Windows and Nearest Competition columns. 
7.	I would like to remove Windows as a Variable because its t test result shows that it is highly not significant in predicting the estimates for sales.
