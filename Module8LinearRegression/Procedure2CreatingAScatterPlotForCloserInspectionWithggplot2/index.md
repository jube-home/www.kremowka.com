---
layout: default
title: "Procedure 2: Creating a Scatter Plot for Closer Inspection with ggplot2"
nav_order: 3
parent: "Module 8: Linear Regression"
grand_parent: Welcome
---

# Procedure 2: Creating a Scatter Plot for Closer Inspection with ggplot2

The scatter plot matrix created in procedure is an extremely useful and informative tool, if lacking beauty.  A package that cannot escape mention for the creation of graphics in R is ggplot2, which is a powerful and flexible graphics package for creating charts and visualisations every bit as beautiful as that which could be found in Excel.  

Start by installing the ggplot package using RStudio:

![img.png](img.png)

Clicking install to download and install the package:

![img_1.png](img_1.png)

Once the packages has been downloaded and installed, reference the package using the library() function and its name ggplot2:

``` r
library(ggplot2)
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

In this example a scatter plot will be created with the Dependent Vector on the y Axis and the Median_4 on the x axis, and initially using just the built in function plot():

``` r
plot(FDX$Median_4,FDX$Dependent)
```

![img_4.png](img_4.png)

The signature of the plot() function is effortless and it is a fantastic extensions to perform quick and exploratory data analysis,  although it may not be visually impressive enough for the purposes of presentations.  qplot() is a function in the ggplot2 package and achieves much the same,  just visually more striking:

``` r
qplot(FDX$Median_4,FDX$Dependent)
```

![img_5.png](img_5.png)

Run the line of script to console:

![img_6.png](img_6.png)

The package ggplot2 provides a plethora of functions that will create rich and visually impressive graphics, from the being able to manipulate colours to correctly titling a plot with the intention of creating graphics fit for publishing.  

The ggplot functionality will be steadily introduced in subsequent procedures although creating visually striking charts for publication is outside the scope of this course.