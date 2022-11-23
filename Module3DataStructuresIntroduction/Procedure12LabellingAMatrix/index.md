---
layout: default
title: "Procedure 12: Labelling a Matrix"
nav_order: 13
parent: "Module 3: Data Structures Introduction"
grand_parent: Welcome
---

# Procedure 12: Labelling a Matrix.

As seen in procedure 24 it is helpful for reference to label a Vector.  It is possible also to label the rows and the columns of a matrix in a similar fashion using the rownames() and colnames() function.

To set column names assign a Vector to the colnames() function, where the colnames() function accepts the matrix as its argument:

``` r
colnames(OverspillMatrix) <- c("Example1","Example2","Example3","Example4")
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

The rownames() function has a similar signature and takes a Vector of row names:

``` r
rownames(OverspillMatrix) <- c("Row1","Row2","Row3")
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

The matrix is now labelled in both directions and can be inspected by typing:

``` r
OverspillMatrix
```

![img_4.png](img_4.png)

Run the line of script to console:

![img_5.png](img_5.png)

