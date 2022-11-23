---
layout: default
title: "Procedure 14: Creating a Factor from a Vector"
nav_order: 15
parent: "Module 3: Data Structures Introduction"
grand_parent: Welcome
---

# Procedure 14: Creating a Factor from a Vector

The factor() function turns a Vector containing character fields into a special structure for categorical variables.  Categorical variables are treated differently in data analysis as conceptually they are pivoted to columns in their own right.

Assume that a Vector of customer genders exists:

``` r
Gender <- c("Male","Female","Female","Male")
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

A standard vector has been created.  To transform this Vector into a Factor, simply pass the Gender Vector as an argument to the factor() function by typing:

``` r
GenderFactor <- factor(gender)
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

It can be observed that the Factor is now available in the environment pane:

![img_4.png](img_4.png)

To view the factor in the console type:

``` r
GenderFactor
```

![img_5.png](img_5.png)

Run the line of script to console:

![img_6.png](img_6.png)

Closer inspection shows that despite there being a vector of the strings Male and Female duplicated,  the Factor has correctly identified there to be two levels of Male and Female.  This procedure is an example of the levels being inferred.  Categorical data will not be treated natively in the predictive analytics tools as follows.