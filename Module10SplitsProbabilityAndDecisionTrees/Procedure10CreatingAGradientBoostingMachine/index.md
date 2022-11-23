---
layout: default
title: "Procedure 10: Creating a Gradient Boosting Machine"
nav_order: 11
parent: "Module 10: Splits, Probability and Decision Trees"
grand_parent: Welcome
---

# Procedure 10: Creating a Gradient Boosting Machine

A relatively underutilised classification tool, which is built upon the concept of boosted decision trees, is the Gradient Boosting Machine, or GBM.  The GBM is a fairly black box implementation of the methods covered thus far, in this module.  The concept of Boosting refers to taking underperformed classifications and singling them out for boosting, or rather creating a dedicated model targeting the weaker performing data.  The GBM is part of the GBM package, as such install that package:

![img.png](img.png)

Click Install to download and install the package:

![img_1.png](img_1.png)

Load the library:

``` r
library(GBM)
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

The warning messages can be ignored as we can be reasonably assured of backward compatibility between the package build and this version of R.

Creating a GBM is similar to the familiar interfaces of regression, except for having a few parameters relating to the taming of the GBM:

``` r
gbm = gbm(Dependent ~., CreditRisk,
n.trees=1000,
shrinkage=0.01,
distribution="gaussian",
interaction.depth=7,
bag.fraction=0.9,
cv.fold=10,
n.minobsinnode = 50
)
```

Run the line of script to console:

![img_4.png](img_4.png)

Run the line of script to console, it may take some time:

![img_5.png](img_5.png)

To review the performance statistics of the GBM, simply recall the model:

``` r
gbm
```

![img_6.png](img_6.png)

Run the line of script to console:

![img_7.png](img_7.png)

The most salient information from this summary is that 1000 iterations were performed, with the cross validation diverging at tree 542.  A visual inspection of the cross validation can be presented by:

``` r
gbm.perf(gbm)
```

![img_8.png](img_8.png)

Run the line of script to console:

![img_9.png](img_9.png)

It can be seen that the line was drawn at the point divergence started:

![img_10.png](img_10.png)

As decision trees can become a little unwieldy, it might be prudent to inspect the relative importance of each of the independent variables with a view to pruning and rerunning the GBM training.  To understand the importance of each Independent Variable, wrap the summary function around the GBM:

``` r
summary(GBM)
```

![img_11.png](img_11.png)

Run the line of script to console:

![img_12.png](img_12.png)

The most useful and important variable is written out first, with the less important being written out last.  This is also displayed in a bar chart giving the overall usefulness of the independent variables at a glance:

![img_13.png](img_13.png)