---
layout: default
title: "Procedure 3: Set a Working Directory"
nav_order: 4
parent: "Module 2: Getting Started with R"
grand_parent: Welcome
---

# Procedure 3: Set a Working Directory

A working directory is where R will look for files during a session.  The files may be the R session, or in subsequent procedures it will be data to be imported and data saved as the result of processing.  

In procedure 2, it was observed that there was a failure when saving the R history, owing to the working directory not being set (rather set incorrectly).  It follows that the working directory need be set.

Start by executing procedure 1 to load the R console.

![img.png](img.png)

To identify the current working directory use the getwd() function, type the script line:

``` r
getwd()
```

![img_1.png](img_1.png)

Execute the command by pressing the Enter key:

![img_2.png](img_2.png)

The current working directory, which is the directory containing the executable, is returned.  Saving files to the same directory as the R software is not desirable, quite beyond it causing errors, and as such, this should be changed to an appropriate directory.

Create a directory to be used throughput these procedures.  In this case the files will be saved to the d:\ in a directory called R:

![img_3.png](img_3.png)

To set this as the working directory in R use the setwd() function with the directory in quotation marks, type:

``` r
setwd("d:/R")
```

![img_4.png](img_4.png)

Press the Enter key to process the line of script:

![img_5.png](img_5.png)

The absence of any error message confirms that the working directory has been changed, although this can be affirmed by executing the getwd() function:

``` r
getwd()
```

![img_6.png](img_6.png)

The working directory is now set to d:\r.

If R is exited, and y is selected to save, it can be observed that there were no errors:

![img_7.png](img_7.png)

Furthermore, it can be seen that the .RHistory file has been saved to the working directory:

![img_8.png](img_8.png)