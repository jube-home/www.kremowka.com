---
layout: default
title: "Procedure 5: Create a Naive Bayesian Network with a Laplace Estimator"
nav_order: 6
parent: "Module 11: Naive Bayesian Classifiers and Laplace Estimator"
grand_parent: Welcome
---

# Procedure 5: Create a Naive Bayesian Network with a Laplace Estimator

To create a Bayesian model with a nominal Laplace estimator of 1, which will mean that in the event that there is nothing it is switch to at least one occurrence in the observation, simply change the parameter value in the training:

SafeBayesianModel <- naiveBayes(CreditRisk,CreditRisk$Dependent,laplace=1)

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

A Bayesian model has been created as SafeBayesianModel.  Recall the model:

``` r
ClassPredictions <- predict(SafeBayesianModel,CreditRisk,type = "class")
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

The de-facto method to appraise the performance of the model would be to create a confusion matrix:

``` r
library(gmodels)
CrossTable(CreditRisk$Dependent, ClassPredictions)
```

![img_4.png](img_4.png)

Run the block of script to console:

![img_5.png](img_5.png)

It can be seen that this naive Bayesian model appears to be startlingly accurate, which stands to reason as the same data is being used to test as was trained.  It follows that this would benefit from an element of cross validation: