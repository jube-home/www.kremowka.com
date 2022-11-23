---
layout: default
title: "Procedure 5: Selecting and Filtering from a numeric Vector"
nav_order: 6
parent: "Module 3: Data Structures Introduction"
grand_parent: Welcome
---

# Procedure 5: Selecting and Filtering from a numeric Vector.

There are a number of ways to specifically extract data from a vector, a process sometimes called subscripting.  In this procedure, the vector created in procedure 21 will be used.  The simplest way to extract data from a vector is to specify the position inside square brackets.  To subscript and retrieve the third value in the vector type:

``` r
SequenceBasic[3]
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

It can be observed that the value at the third position in the SequenceBasic vector has been returned.  Alternatively, specifying a negative value of 3 would return everything except the third position:

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

It can be observed that the third position of the vector has been excluded in the output.

Far more powerful is the ability to select from vectors based upon a logical statement, such as all values > 5:

``` r
SequenceBasic[SequenceBasic > 5]
```

![img_4.png](img_4.png)

Run the line of script to console:

![img_5.png](img_5.png)

It can be seen that only values greater than five have been returned.  The notion of selecting from a vector based on logical conditions further introduces operators:

* & And.
* | Or.
* ! Not.

To create more discriminating selection from a vector, where the value must be > 2 and less than 5, type:

``` r
SequenceBasic[SequenceBasic > 2 & SequenceBasic <5]
```

![img_6.png](img_6.png)

Run the line of script to the console:

![img_7.png](img_7.png)

It can be seen that only the two values between 2 and 5 have been returned.