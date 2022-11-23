---
layout: default
title: "Procedure 20: Saving .Rdata to file"
nav_order: 21
parent: "Module 3: Data Structures Introduction"
grand_parent: Welcome
---

# Procedure 20: Saving .Rdata to file

Machine learning is predominantly a challenge of data abstraction – this is the shaping and moulding of data – and presenting it to advanced machine learning algorithms on a commodity basis.  It follows that upon having spent time and effort creating an elaborate Data Frame,  it likely that it will need to be saved for future use (if only to avoid the computational expense of recreating it).

The save() function exists for the purpose of saving most objects that can be created and populated with data to a file in the working directory.  It is a very important part to deploying models on a real-time basis.

To save the Data Frame LabeledDataFrame and BucketList to a specified file by the name of "Example.RData":

``` r
save(LabeledDataFrame,BucketList,file = "Example.RData")
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

A file titled Example.RData is not written out to the Working Directory.  To remind the working directory:

``` r
getwd()
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

Having identified the working directory, navigate to the same in windows explorer:

![img_4.png](img_4.png)

The saved file is clearly visible in this directory ready for real-time deployment or being reloaded to an R session.