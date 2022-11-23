---
layout: default
title: "Procedure 8: Using the predict function for a one way linear regression one"
nav_order: 9
parent: "Module 8: Linear Regression"
grand_parent: Welcome
---

# Procedure 8: Using the predict function for a one way linear regression one

Deploying a linear regression model manually is rather simple, however, there is an even simpler method available in calling the predict() function which takes a model and a data frame as its parameter,  returning a prediction vector.

``` r
AutomaticLinearRegression <- predict.lm(LinearRegression,FDX)
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

Add the newly created vector to the FDX data frame:

``` r
FDX <- mutate(FDX, AutomaticlLinearRegression)
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

To view the last two columns of the data frame, containing a manually derived prediction and automatically derived prediction:

``` r
View(FDX[,203:204])
```

![img_4.png](img_4.png)

Run the line of script to console:

![img_5.png](img_5.png)

The manual and automatic prediction shown side by side are identical to each other.  It follows that the automatic prediction is a much more concise means to execute the prediction based upon a linear regression model created in R:

![img_6.png](img_6.png)