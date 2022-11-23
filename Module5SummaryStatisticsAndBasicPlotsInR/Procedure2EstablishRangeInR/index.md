---
layout: default
title: "Procedure 2: Establish Range in R"
nav_order: 3
parent: "Module 5: Summary Statistics and Basic Plots in R"
grand_parent: Welcome
---

# Procedure 2: Establish Range in R

To establish the range of the Interim_Close in the AAPL data frame use the min() function typing:

``` r
min(AAPL$Interim_Close)
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

It can be seen that the smallest value in the Interim_Close vector of the AAPL data frame is 50.67, to retrieve the largest value use the max() function by typing:

``` r
range(AAPL$Interim_Close)
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

Run the line of script to console:

![img_4.png](img_4.png)

To establish the range value subtract the largest value from the smallest value which can be achieved by using the diff() function on the vector returned from the range() function as:

``` r
diff(range(AAPL$Interval_Close))
```

![img_5.png](img_5.png)

Run the line of script to console:

![img_6.png](img_6.png)

It can be seen that the range has been returned as being 651.43.