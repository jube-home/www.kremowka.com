---
layout: default
title: "Procedure 7: Recalling a Neural Network with R"
nav_order: 8
parent: "Module 14: Deep Learning with H20"
grand_parent: Welcome
---

# Procedure 7: Recalling a Neural Network with R

Once a model is trained in H2O it can be recalled very gracefully with the predict() function of the H2O package.  It is a simple matter of passing the trained model and the hex dataframe to be used for recall:

``` r
Scores <- h2o.predict(Model,CVHex.hex)
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

A progress bar is broadcast from the H2O server and will be written out to the console.  To review the output, enter the object:

``` r
Scores
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

The Scores output appears similar to a matrix, but it has created a vector which details the actual prediction for a record, hence, this can be subset to a final vector detailing the predictions:

``` r
Predict <- Scores[1]
```

![img_4.png](img_4.png)

Run the line of script to console:

![img_5.png](img_5.png)

The Predict vector can be compared to the Dependent vector of the CV dataframe in the same manner as previous models within R to obtain Confusion Matrices as well a ROC curves.