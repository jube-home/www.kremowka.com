---
layout: default
title: "Procedure 2: Quickly Creating a Line Chart with qplot()"
nav_order: 3
parent: "Module 6: ggplot2 Rapid Exploration"
grand_parent: Welcome
---

# Procedure 2: Quickly Creating a Line Chart with qplot()

Displaying a stock price over time is a convenient example to show the functionality of qplot when used to make a line chart.  In this example, the FedEx stock price is going to be plotted over time.  As with the scatter plot example, the qplot function takes two vectors, however, the geom parameter will be used to specify the type of chart, in this case "line".  To create a time series line chart, pass a date (Interim_Date) and the price (Interim_Close):

``` r
qplot(FDX$Interim_Buffer_Date,FDX$Interim_Close,geom="line")
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

It can be observed that the chart has been rendered to the plots section of RStudio:

![img_2.png](img_2.png)

This procedure should exhibit that qplot has default of a scatter chart, however it can be easily changed to other types by varying the geom parameter.