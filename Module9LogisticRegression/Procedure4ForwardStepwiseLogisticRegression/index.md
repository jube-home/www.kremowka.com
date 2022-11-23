---
layout: default
title: "Procedure 4: Forward Stepwise Logistic Regression"
nav_order: 5
parent: "Module 9: Logistic Regression"
grand_parent: Welcome
---

# Procedure 4: Forward Stepwise Logistic Regression

As procedure 97 alludes, whereas the linear regression function in R was lm(), the logistic regression function is glm(), with supplementary parameters specifying the family as being a binomial distribution (which is a stalwart distribution for classification problems).  As in procedure 89 which create a linear regression model, the syntax is very similar to create a logistic regression model, albeit including the family argument:

``` r
LogisticRegressionModel <- glm(Dependent ~ Count_Unsafe_Terminals_1_Day,data=FraudRisk,family="binomial")
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

As with a lm() type model, the summary() function can return the model output:

``` r
summary(LogisticRegressionModel)
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

As with models created using the lm() function, the summary is somewhat inadequate to get the coefficients with correct precision, notwithstanding that the predict.glm() function will be used for recall:

``` r
coefficients(LogisticRegressionModel)
```

![img_4.png](img_4.png)

Run the line of script to console to output the coefficients for a manual deployment of the logistic regression model:

![img_5.png](img_5.png)

This procedure would naturally lead into a stepwise multiple logistic regression model, and in this example a factor as created in preceding procedures will be added with the assumption that it is the next strongest correlating factor:

![img_6.png](img_6.png)

Run the line of script to console:

![img_7.png](img_7.png)

Write out the coefficients to observe the treatment of each different state inside the factor TypeFactor:

![img_8.png](img_8.png)