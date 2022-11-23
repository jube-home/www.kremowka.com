---
layout: default
title: "Procedure 12: Specifying columns of a Data Frame to return"
nav_order: 13
parent: "Module 4: Loading, Shaping and Merging Data"
grand_parent: Welcome
---

# Procedure 12: Specifying columns of a Data Frame to return

The select() function returns just the columns specified after the data frame.  In this example, the AAPL data frame will be have some columns truncated leaving only the columns Interim_Buffer_Date and Interim_Close:

``` r
AAPL <- select(AAPL,Symbol,Interim_Buffer_Date,Interim_Close)
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

View the data frame:

``` r
View(AAPL)
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

It can be observed that the data frame has discarded columns that were not specified explicitly.