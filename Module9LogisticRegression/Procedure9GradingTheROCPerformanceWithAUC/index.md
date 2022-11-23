---
layout: default
title: "Procedure 9: Grading the ROC Performance with AUC"
nav_order: 10
parent: "Module 9: Logistic Regression"
grand_parent: Welcome
---

# Procedure 9: Grading the ROC Performance with AUC

Visually the plot created suggests a that the model created has some predictive power.  A more succinct method to measure model performance is the Area Under Curve statistics which can be calculated with ease by requesting "auc" as the measure to the performance object:

``` r
AUC <- performance(ROCRPredictions,measure = "auc")
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

To write out the contents of the AUC object:

``` r
AUC
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

The value to gravitate towards is the y.values,  which will have a value ranging between 0.5 and 1:

![img_4.png](img_4.png)

In this example, the AUC value is 0.827767 which suggests that the model has an excellent utility. By way of grading, AUC scores would correspond:

* A: Outstanding > 0.9
* B: Excellent > 0.8 and <= 0.9
* C: Acceptable > 0.7 and <= 0.8
* D: Poor > 0.6 and <= 0.7
* E: Junk > 0.5 and <= 0.6