---
layout: default
title: "Procedure 2: Extracting a substring from a string, testing logically and presenting for machine learning"
nav_order: 3
parent: "Module 4: Loading, Shaping and Merging Data"
grand_parent: Welcome
---

# Procedure 2: Extracting a substring from a string, testing logically and presenting for machine learning

In Horizontal Abstraction, it is quite common to have the requirement to inspect a string of data looking for an occurrence (or pattern) and return a logical value that can be used in machine learning.

In this example, a string will be inspected and return a 1 in the event that the string "Richard" is present.

Firstly, create a vector of name strings by typing:

``` r
Names <- c("Richard","Robert","Reinhard","Raymond","Richardino","Richardo")
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

Use the substr() function to create a vector of the first 7 characters of the value contained in the Names vector,  by typing:

``` r
NamesSubstr <= substr(Names,1,7)
```

![img_2.png](img_2.png)

Write the NamesSubstr vector:

``` r
NamesSubstr
```

![img_3.png](img_3.png)

Run the line of script to console:

![img_4.png](img_4.png)

The question being posed is whether the first characters of the name is equal to "Richard".  To perform this evaluation, create a logical vector from the NamesSubstr vector by typing:

``` r
NamesSubstrLogical <- NamesSubstr == "Richard"
```

![img_5.png](img_5.png)

Notice how a double equals sign is used to eliminate confusion between evaluation and assignment. 

Run the line of script to console:

![img_6.png](img_6.png)

Write the logical vector out to console by typing:

``` r
NamesSubstrLogical
```

![img_7.png](img_7.png)

Run the line of script to console:

![img_8.png](img_8.png)

The character notion of TRUE or FALSE cannot be used in machine learning readily (you can’t multiply by text) and it follows that these values should be converted to a numeric value using the as.numeric() function,  typing:

``` r
NamesSubstrLogicalNumeric <- as.numeric(NamesSubstrLogical)
```

![img_9.png](img_9.png)

Run the line of script to console:

![img_10.png](img_10.png)

Write the newly created vector to console by typing:

![img_11.png](img_11.png)

Run the line of script to console:

![img_12.png](img_12.png)

A more concise line of script nesting the functions might be:

``` r
NamesSubstrLogicalNumericNested <- as.numeric(substr(Names,1,7) == "Richard")
```

![img_13.png](img_13.png)

An alternative approach might be converting the logical vector to a factor as explained elsewhere.
