---
layout: default
title: "Procedure 18: Remove Variables in R"
nav_order: 19
parent: "Module 2: Getting Started with R"
grand_parent: Welcome
---

# Procedure 18: Remove Variables in R

In the event that long and complex scripts are being processed, where the objects might be using a substantial amount of memory (such as a large table from a database), it may be prudent to remove the objects when the script no longer needs it.

To remove an object, the remove() function is used taking an argument as the name of the variable to be removed.  In this example, the String variable will be removed.  Type:

``` r
remove("String")
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

It can be seen that the String variable no longer appears in the environment pane:

![img_2.png](img_2.png)

Naturally the variable will not be available in the session upon inspection of the ls() function.  Type:

``` r
ls()
```

![img_3.png](img_3.png)

Run the line of script to console:

![img_4.png](img_4.png)

It can be observed that the return is now minus the String variable.