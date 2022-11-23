---
layout: default
title: "Procedure 16: Create a logical variable by assignment"
nav_order: 17
parent: "Module 2: Getting Started with R"
grand_parent: Welcome
---

# Procedure 16: Create a logical variable by assignment

Logical variables are True or False values which are derived by logical assignment.  To create a logical variable as the result of an evaluation assignment, start by creating a variable x by typing:

``` r
x <- 1
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

Create another variable y by typing:

``` r
y <- 2
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

The logical variable will be created as the result of comparing one variable to another, in this case, questioning if x is greater than y.  Type:

``` r
Logical <- x > y
```

![img_4.png](img_4.png)

Run the line of script to the console:

![img_5.png](img_5.png)

It can be seen that the variable Logical has been created and is available in the Environment pane:

![img_6.png](img_6.png)

Naturally, the variable can also be referenced via simply typing into the script editor:

``` r
Logical
```

![img_7.png](img_7.png)

Run the script to console:

![img_8.png](img_8.png)

It can be seen that the variable has been written out as FALSE, in this instance, with the opposing value being TRUE.  Using the mode() function,  typing into the script editor:

``` r
mode(Logical)
```

![img_9.png](img_9.png)

Run the script to console:

![img_10.png](img_10.png)

It can be seen that the variable writes out as being of type logical.

