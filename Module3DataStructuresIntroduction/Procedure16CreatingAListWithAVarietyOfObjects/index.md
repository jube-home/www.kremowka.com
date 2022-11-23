---
layout: default
title: "Procedure 16: Creating a list with a variety of objects"
nav_order: 17
parent: "Module 3: Data Structures Introduction"
grand_parent: Welcome
---

# Procedure 16: Creating a list with a variety of objects

A list is very similar to a Vector except it allows the storage of more than one type of object,  whereas a Vector must be the same type.  In the procedures preceding, many objects have been created.  A list can bring these objects together despite them being of radically different types.

The list() function, used to create lists, is very similar to that of the c() function except it has a broader ability to specify object names at creation.   To create a list aggregating some objects created in the preceding procedures:

``` r
BucketList <- list(TempsExample = TempsFactors,GenderExample = GenderFactors,MatrixExample = Matrix3Row,VectorExample = Ages)
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

It can be seen that the list is now available in the environment pane:

![img_2.png](img_2.png)

Specifically it is possible,  by clicking on the play icon,  to expand the list and inspect the objects inside the list in turn:

![img_3.png](img_3.png)

To write out the entire contents of the list to the console type:

``` r
BucketList
```

![img_4.png](img_4.png)

Run the line of script to console. It can be seen that each item of the list and its contents have been written out in turn.