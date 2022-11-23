---
layout: default
title: "Procedure 11: List all Functions in a Package"
nav_order: 12
parent: "Module 2: Getting Started with R"
grand_parent: Welcome
---

# Procedure 11: List all Functions in a Package

Once a package is loaded, beyond using the help as detailed in procedure 8, an understanding of all the functions available to the package can be obtained.   Although a script active, console passive approach is advocated this procedure is one of the few occasions where it is more appropriate to use the console directly rather than clutter up the script.

Click on the console window in the bottom left hand corner of RStudio:

![img.png](img.png)

Type directly into the console:

``` r
ls("package:ggplot2")
```

![img_1.png](img_1.png)

Press the Enter key to execute the script:

![img_2.png](img_2.png)

A list of all functions in the package is returned.