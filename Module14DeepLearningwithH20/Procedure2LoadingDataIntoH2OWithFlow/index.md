---
layout: default
title: "Procedure 2: Loading Data into H2O with Flow"
nav_order: 3
parent: "Module 14: Deep Learning with H20"
grand_parent: Welcome
---

# Procedure 2: Loading Data into H2O with Flow

In this example a logistic regression model will be created, using Flow, achieving the same results as achieved in the GLM functions of R and Exhaustive.

In the Flow user interface, start by navigating:

``` r
Flow >>> New Flow
```

![img.png](img.png)

If prompted to create a new workbook, affirm this:

![img_1.png](img_1.png)

To add a cell for the importing of data, navigate to:

``` r
Data >>> Import Files
```

![img_2.png](img_2.png)

It can be seen that Import Files Cell has been added to the Flow:

![img_3.png](img_3.png)

In the Search dialog box, enter the location of the FraudRisk.csv file until a drop down is populated, for example:

![img_4.png](img_4.png)

Click on the Search Icon to bring back the contents of this directory:

![img_5.png](img_5.png)

Click on the file or plus sign to add the file to the cell:

![img_6.png](img_6.png)

Click the Import Button to import the file to H2O:

![img_7.png](img_7.png)

Note that the file is not parsed to the H2O column compressed format, known as Hex.  To achieve parsing, simply click the button titled 'Parse These Files':

![img_8.png](img_8.png)

The next screen allows for the specification and data types to be more robustly configured.  In this example, a cursory check to ensure that the data types are correct is sufficient:

![img_9.png](img_9.png)

Upon satisfaction, click parse to mount the dataset in H20 as Hex:

![img_10.png](img_10.png)

A background job will start the process of transforming the data from FraudRisk.csv to the H2O hex format:

![img_11.png](img_11.png)

H2O supports the concept of training and validation datasets robustly, henceforth the hex file needs to be split into training and validation.  To split a Hex frame, navigate to:

``` r
Data >>> Split Frame
```

![img_12.png](img_12.png)

Click on the menu item to create the split data frame cell:

![img_13.png](img_13.png)

Select the frame to be split, in this case FraudRisk.hex:

![img_14.png](img_14.png)

The default frame split is 75% by 25%, confirm this by clicking the Create button:

![img_15.png](img_15.png)

There now exists two frames in the flow, the smaller of which will be used for validation:

![img_16.png](img_16.png)