---
layout: default
title: "Procedure 7: Browsing and Installing Packages"
nav_order: 8
parent: "Module 2: Getting Started with R"
grand_parent: Welcome
---

# Procedure 7: Browsing and Installing Packages

For the purposes of these procedures all external packages will be sourced from CRAN via Rstudio.   In this procedure the graphics and plotting package titled ggplot2 will be installed.

Navigate to the Packages pane, clicking the tab if necessary, in the bottom right hand corner of RStudio:

![img.png](img.png)

Click on the button Install:

![img_1.png](img_1.png)

The Install Package dialog box will display,  defaulting to the CRAN mirror:

![img_2.png](img_2.png)

To search for a package by name, type the name in the package textbox:

``` r
ggplot2
```

![img_3.png](img_3.png)

Autocomplete will suggest two packages having reviewed potential matched on CRAN,  accept \ click on the suggested ggplot2:

![img_4.png](img_4.png)

Always keep the Install Dependencies button as checked.  Clicking install will send commands to the console to install the packages:

![img_5.png](img_5.png)

The package is now installed.  

Executing the search() function it can be observed however that the package appears not to be loaded:

![img_6.png](img_6.png)