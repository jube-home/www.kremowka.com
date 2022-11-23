---
layout: default
title: "Procedure 14: Merging a Data Frame"
nav_order: 16
parent: "Module 4: Loading, Shaping and Merging Data"
grand_parent: Welcome
---

# Procedure 14: Merging a Data Frame

Repeat the process to create a data frame, this time creating a data frame called Descriptions from the table EOD_Descriptions by typing:

``` r
Descriptions <- sqlQuery(Connection,"select * from EOD_Desccriptions")
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

View the Descriptions data frame by typing:

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

It can be seen that symbol column is common between the AAPL table and the Descriptions table.
The task in this procedure is to merge the data frames together on the Symbol identifier, which will then provide a description next to each and every record in the AAPL dataset.  The inner_join() function seeks to bring together all records where the key in one data frame is present in the other.

To join two data frames in this manner type:

``` r
AAPL <- inner_join(AAPL,Descriptions,ID = "Symbol")
```

![img_4.png](img_4.png)

Run the line of script to console:

![img_5.png](img_5.png)

Notice that an error relating to levels has been produced, this is owing to there being a disparity in the number of records in one table as opposed to the next.  Inspect the new dataset by typing:

``` r
View(AAPl)
```

![img_6.png](img_6.png)

It can be seen that the description field from the Descriptions Data Frame has been duplicated across each record in the AAPL Data Frame, as would be expected of an Inner Join in a database:

![img_7.png](img_7.png)