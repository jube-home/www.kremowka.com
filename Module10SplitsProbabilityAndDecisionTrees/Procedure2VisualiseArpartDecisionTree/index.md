---
layout: default
title: "Procedure 2: Visualise a rpart Decision Tree"
nav_order: 3
parent: "Module 10: Splits, Probability and Decision Trees"
grand_parent: Welcome
---

# Procedure 2: Visualise a rpart Decision Tree

Once familiar with the output of a regression tree, it becomes an informative means to create business rules. Quite often however, for the purposes of communication, it is more satisfying to create a visualisation.  A package called rpart.plot is available for the purposes of translating regression trees to a visualisation.  Start by installing the rpart.ploy package:

![img.png](img.png)

Click install to download and install the package:

![img_1.png](img_1.png)

Reference the library:

``` r
library(rpart.plot)
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

To transpose the Regression Tree to a plot, simply pass it as an argument to the rpart.plot() function:

``` r
rpart.plot(RegressionTree)
```

![img_4.png](img_4.png)

Run the line of script to console:

![img_5.png](img_5.png)

It can be seen that a complex visualisation has been created in the plots window of R Studio:

![img_6.png](img_6.png)

The visualisation is exceptionally hard to interpret for a large regression tree; hence it will likely need to be exported to a PDF or Image file to use a zoom function:

![img_7.png](img_7.png)