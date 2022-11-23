---
layout: default
title: "Procedure 6: Creating a One Way Linear Regression Model"
nav_order: 7
parent: "Module 8: Linear Regression"
grand_parent: Welcome
---

# Procedure 6: Creating a One Way Linear Regression Model

In procedure 88 the lm() function was used inside the stat_smooth() function of ggplo2 to create a linear regression solution,  rather line of best fit. Naturally the lm() function can also be used to create linear regression model which can be deployed as a predictive model in its own right.

To create a linear regression model with one dependent variable and one independent variable:

``` r
LinearRegression <- lm(Dependent ~ Median_4,FDX)
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

Once the model has been computed it can be output:

LinearRegression

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

The most vital aspects of the solution are written out chiefly the Intercept and Coefficient for Median_4.  Notably there is no statistical measures to appraise the overall worth of the solution.

The summary() function can be used to expand on the validity and performance of the model:

``` r
summary(LinearRegression)
```

![img_4.png](img_4.png)

Run the line of script to console:

![img_5.png](img_5.png)

A more traditional Linear Regression model has now been written out.   It is worth checking the precision of the coefficients to ensure that they have not been truncated, as this can lead to a profound change in the predicted values:

``` r
coeefeicents(LinearRegression)
```

![img_6.png](img_6.png)

Run the line of script to console:

![img_7.png](img_7.png)

It can be seen that the coefficients written out have rather more decimal places, or precision, which will be extremely important when seeking to make accurate predictions.