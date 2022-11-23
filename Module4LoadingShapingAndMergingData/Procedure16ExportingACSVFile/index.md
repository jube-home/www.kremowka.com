---
layout: default
title: "Procedure 16: Exporting a csv file"
nav_order: 18
parent: "Module 4: Loading, Shaping and Merging Data"
grand_parent: Welcome
---

# Procedure 16: Exporting a csv file

By this stage a large amount of manipulation has been performed on the AAPL data frame and it bears little resemblance to that which was originally loaded.  Exporting data frames from R is a common requirement to communicate work product to business users.  In general, if there is an object to read something into R, then there is the near equivalent to write from R.  In this example, the write.csv function will be used to write the AAPL dataframe to a csv file, in the file system:

``` r
write.csv(AAPL,file="AAPL.csv")
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

To identify the location of the working directory, use the getwd() function:

``` r
getwd()
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

Open the directory in windows explorer:

![img_4.png](img_4.png)

Opening the file, it can be seen that the data frame has been reliably exported:

![img_5.png](img_5.png)