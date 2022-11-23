---
layout: default
title: "Procedure 6: Setting Vector Labels or Names"
nav_order: 7
parent: "Module 3: Data Structures Introduction"
grand_parent: Welcome
---

# Procedure 6: Setting Vector Labels or Names

Selecting from a character vector follows the same pattern,  in so far as the criteria sits inside [] square brackets and allows for the specific selection of values or the specific exclusion of values.  Create a character vector by typing numbers,  henceforth ages:

``` r
Ages <- c(22,23,28)
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

It is possible to add labels to the entries in the vector using the names() function, similar to column headers in an Excel spreadsheet.   The label 22 is Tom’s Age, 23 is Harries Age and lastly 28 is Dicks Age.  To add labels to each Vector value, type:

``` r
names(Ages) <- c("Tom","Harry","Dick")
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

It can be observed that the Vector in the environment pane is now marked as being a ‘Named’ vector:

![img_4.png](img_4.png)

Outputting the Vector to console, type:

![img_5.png](img_5.png)

Run the line of script to console:

![img_6.png](img_6.png)

It can be observed that the vector more closely resembles the row of a spreadsheet.  The names function will be used more extensively when aggregating Vectors into a Matrix, for the time being however, it will be used to allow for the selection of just that individuals Age.