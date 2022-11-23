---
layout: default
title: "Procedure 10: Combine Vectors to make a Matrix with rbind"
nav_order: 11
parent: "Module 3: Data Structures Introduction"
grand_parent: Welcome
---

# Procedure 10: Combine Vectors to make a Matrix with rbind

Whereas procedure 26 brought vectors together as columns,   rbind() can bring vectors together as rows.  Start by creating two vectors in a script block:

``` r
Row1 <- c(1,2,3,4,5,6,7,8,9,10)
Row2 <- c(10,20,30,40,50,60,70,80,90,100)
Row3 <- c(100,200,300,400,500,600,700,800,900,1000)
```

![img.png](img.png)

Run the script block to console:

![img_1.png](img_1.png)

To bind the vectors as rows use the rbind() function:

``` r
Matrix3Row <- c(Row1,Row2,Row3)
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

The matrix can be viewed by typing:

``` r
Matrix3Row
```

![img_4.png](img_4.png)

Run the line of script to console:

![img_5.png](img_5.png)