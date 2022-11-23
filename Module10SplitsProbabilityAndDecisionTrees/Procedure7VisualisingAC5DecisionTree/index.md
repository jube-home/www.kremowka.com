---
layout: default
title: "Procedure 7: Visualising a C5 Decision Tree"
nav_order: 8
parent: "Module 10: Splits, Probability and Decision Trees"
grand_parent: Welcome
---

# Procedure 7: Visualising a C5 Decision Tree

To visualise a C5 Decision tree, the plot() function from the R base functions can be used, passing the C5 decision tree model as the argument:

``` r
plot(C50Tree)
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

It can be seen that a visualisation has been written out to the plots pane:

![img_2.png](img_2.png)

If the tree is very large, then the zoom feature will need to be used to ensure that the plot fits the screen.  Even with zoom, it is possibly more appropriate to communicate the product of C5 decision trees as a list of rules.