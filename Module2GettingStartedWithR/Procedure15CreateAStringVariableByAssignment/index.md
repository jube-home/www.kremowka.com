---
layout: default
title: "Procedure 15: Create a string variable by assignment"
nav_order: 16
parent: "Module 2: Getting Started with R"
grand_parent: Welcome
---

# Procedure 15: Create a string variable by assignment

Strings in R are surrounded by double quotation marks yet the assignment procedure is the same as numeric assignment.  Start by creating a new line in the script editor and typing:

``` r
Char <- "Test"
```

![img.png](img.png)

Run the script to console:

![img_1.png](img_1.png)

The new String value is written to the Environment pane.  The variable is addressable from the script by typing the variable:

``` r
String
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

Validate the variable type by using the mode() function. Type into the script pane:

``` r
mode(String)
```

![img_4.png](img_4.png)

Run the line of script to console:

![img_5.png](img_5.png)

It can be observed that the data type was defined as character upon assignment.