---
layout: default
title: "Procedure 13: Unloading a Package"
nav_order: 14
parent: "Module 2: Getting Started with R"
grand_parent: Welcome
---

# Procedure 13: Unloading a Package

Navigate to the end of the script and create a new line:

![img.png](img.png)

Type the detach() function as:

``` r
detach("package:ggplot2", unload = TRUE)
```

![img_1.png](img_1.png)

Run the line of script to the console:

![img_2.png](img_2.png)

The package has now been removed from the R session and the script is essentially, tidying itself up.