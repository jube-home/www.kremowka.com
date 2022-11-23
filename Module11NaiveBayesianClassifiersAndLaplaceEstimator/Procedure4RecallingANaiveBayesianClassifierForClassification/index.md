---
layout: default
title: "Procedure 4: Recalling a Naive Bayesian Classifier for Classification"
nav_order: 5
parent: "Module 11: Naive Bayesian Classifiers and Laplace Estimator"
grand_parent: Welcome
---

# Procedure 4: Recalling a Naive Bayesian Classifier for Classification

To recall the pivotal classification, rather than recall P for each class and drive it from the larger of the values, the type class can be specified:

``` r
ClassPredictions <- predict(BayesianModel,CreditRisk,type = "class")
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

Merge the classification predictions into the CreditRisk data frame, specifying the dply library also:

``` r
library(dplyr)
CreditRisk <- mutate(CreditRisk, ClassPredictions)
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

Viewing the CreditRisk data frame:

View(CreditRisk)

![img_4.png](img_4.png)

Run the line of script to console:

![img_5.png](img_5.png)

Scroll to the last column in the RStudio viewer to reveal the classification for each record:

![img_6.png](img_6.png)