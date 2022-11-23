---
layout: default
title: "Procedure 3: Recalling a rpart() Decision Tree"
nav_order: 4
parent: "Module 10: Splits, Probability and Decision Trees"
grand_parent: Welcome
---

# Procedure 3: Recalling a rpart() Decision Tree

As with regression and most of the predictive analytics tools presented in this document, the predict() function can take the RegressionTree object in conjunction with a data frame,  then return the predictions.  To create predictions using the RegressionTree model and the FDX dataset:

``` r
RegressionTreePredictions <- predict(RegressionTree,FDX)
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

Merge the newly created vector into the FDX data frame for completeness:

``` r
library(dplyr)
FDX <- mutate(FDX, RegressionTreePredictions)
```

![img_2.png](img_2.png)

Run the block of script to console:

![img_3.png](img_3.png)