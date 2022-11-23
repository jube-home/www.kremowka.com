---
layout: default
title: "Procedure 4: Establish the Mean and Median in R"
nav_order: 5
parent: "Module 5: Summary Statistics and Basic Plots in R"
grand_parent: Welcome
---

# Procedure 4: Establish the Mean and Median in R

The Mean and Median are a way to measure the central tendency of a vector.  The mean, commonly called the average, is calculated by summing up all of the values in a vector the dividing it by the count of values in the vector (i.e. 100 + 200 + 300 / 3).  The function mean() performs the calculation on a vector by typing:

``` r
mean(AAPL$Interim_Close)
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

The mean, or average, is output as 251.8668.  The median on the other hand is absolute middle of a histogram and can be calculated using the median() function:

``` r
median(AAPL$Interim_Close)
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

It can be observed that the median, the value that could be considered the centre of the distribution, is 171.195.  Taken together with procedure 57, all the values are present to create a box and whiskers plot as an alternative to a histogram as a means to understand the spread of data.