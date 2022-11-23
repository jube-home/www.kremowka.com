---
layout: default
title: "Procedure 2: Perform Vector Arithmetic"
nav_order: 3
parent: "Module 3: Data Structures Introduction"
grand_parent: Welcome
---

# Procedure 2: Perform Vector Arithmetic

A variety of arithmetic operators can be used against vectors such as:

* + Addition
* - Subtraction
* * Multiplication
* / Division
* ^ Power
* %% mod

In this example, a numeric Vector will be multiplied by 2.  Start by creating a Vector, type:

``` r
Multiply <- c(1,2,3,4,5)
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

In this example, multiply the vector by 2.   Type:

``` r
Multiply * 2
```

![img_2.png](img_2.png)

Run the line of script to console to write out the new vector:

![img_3.png](img_3.png)

It can be observed that each position in the vector has been multiplied by the value of 2.  It is also possible to multiple by another vector.  Create another vector by typing:

``` r
MultiplyBy <- c(5,4,3,2,1)
```

![img_4.png](img_4.png)

Then multiply the existing vector Multiply by the new vector MultiplyBy by typing:

``` r
Multiply * MultiplyBy
```

![img_5.png](img_5.png)

Run the line of script to console:

![img_6.png](img_6.png)

It can be observed that for each position in the vector, the value in that position has been multiplied by the same position in the other vector.  Think of this as the equivalent of filling down in an Excel spreadsheet.