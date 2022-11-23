---
layout: default
title: "Procedure 1: Install H2O package, instantiate and browse to the Flow User Interface"
nav_order: 2
parent: "Module 14: Deep Learning with H20"
grand_parent: Welcome
---

# Procedure 1: Install H2O package, instantiate and browse to the Flow User Interface

Even though H2O is server software and runs externally to R, it can be installed and initialised from with R.  Installing the entire H2O server is no more complex than installing any other R package.

To install H20, use RStudio and begin by installing the H20 package:

![img.png](img.png)

Wait for the installation to complete, although this will take a little bit longer than most packages as it is big:

Load the H2O package by typing:

``` r
library(h2o)
```

![img_1.png](img_1.png)

Run the line of script to console:

![img_2.png](img_2.png)

The H2O server needs to be started externally, but this can be achieved through a helper function available to the H2O library.  To start the H2O server, use the h2o.init function with the default parameters (i.e. no parameters):

``` r
H2oServer <- h2o.init()
```

![img_3.png](img_3.png)

Run the line of script to console and wait for confirmation to be provided that the h2o server has been started externally to R:

![img_4.png](img_4.png)

The h2o server acts as a web server which serves up the Flow application. To navigate to the Flow application, open a browser such as Chrome:

![img_5.png](img_5.png)

Navigate to the URL: http://localhost:54321

![img_6.png](img_6.png)

The H2o server is now installed and available for use via the Flow user interface, API or R commands.