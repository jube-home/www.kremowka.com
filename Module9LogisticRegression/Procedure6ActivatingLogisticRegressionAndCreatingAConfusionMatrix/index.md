---
layout: default
title: "Procedure 6: Activating Logistic Regression and Creating a Confusion Matrix"
nav_order: 7
parent: "Module 9: Logistic Regression"
grand_parent: Welcome
---

# Procedure 6: Activating Logistic Regression and Creating a Confusion Matrix

A logistic regression model outputs values between – 5 and +5, representing zero probability to 100% percent probability.  Zero would represent a 50/50 probability, anything greater than zero would denote the outcome being more likely than not.

In this example, suppose that activation is to take place based upon the balance of probabilities and anything greater than 0 should be considered as being predicted, in this example, as fraud.  The ifelse() function can facilitate the creation of an activation function:

``` r
ActivateAutomaticLogisticRegression <- ifelse(AutomaticLogisticRegression > 0,1,0)
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

For completeness merge the Activated Logistic Regression model into the fraud risk data frame:

``` r
FraudRisk <- mutate(FraudRisk, ActivateAutomaticLogisticRegression)
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

Run the line of script to console to output the confusion matrix:

![img_4.png](img_4.png)

In this example, it can be seen that of 901 records in total, 576 were judged to be fraudulent by the model and were in fraudulent in actuality, some 63.9% a figure for which improvement should be sought via stepwise logistic regression.  

The process of calculating the performance of the confusion matrix in this manner is quite laborious and there exist several packages that help layout the confusion matrix with more readily available performance measures.  Install the gmodels package:

![img_5.png](img_5.png)

Click install to both download and install:

![img_6.png](img_6.png)

Once the gmodels library is installed it needs to be referenced.  To create the confusion matrix, the line of script resembles the table() function almost absolutely, except making use of the CrossTable() function of the gmodels package:

``` r
library("gmodels")
CrossTable(FraudRisk$Dependent, FraudRisk$ActivateAutomaticLogisticRegression)
```

![img_7.png](img_7.png)

Run the line of script to console:

![img_8.png](img_8.png)

It can be seen that a confusion matrix has been created in much the same manner except for it has created the summary statistics across both axis of the table.