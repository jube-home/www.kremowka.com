---
layout: default
title: "Procedure 4: Quickly Creating a Histogram with qplot()"
nav_order: 5
parent: "Module 6: ggplot2 Rapid Exploration"
grand_parent: Welcome
---

# Procedure 4: Quickly Creating a Histogram with qplot()

The qplot() histogram bears resemblance to the hist() function,  being called almost identically:

``` r
qplot(Boston$PerCapitaCrimeRate)
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

It can be seen that an error message has been created suggesting that the bin width is too wide, which is clearly the case in the plot being written out with a very wide scale:

![img_2.png](img_2.png)

Specifying the binwidth parameter of the qplot function solves the issue of their being too many bins by widening the size of the bins:

``` r
qplot(Boston$PerCapitaCrimeRate,binwidth=10)
```

![img_3.png](img_3.png)

Run the line of script to console:

![img_4.png](img_4.png)

It can be seen that a histogram has been plotted in RStudio, with fewer bars owing to the distances for the bars being wider:

![img_5.png](img_5.png)