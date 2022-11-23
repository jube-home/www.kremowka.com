---
layout: default
title: "Procedure 4: Recalling a Logistic Regression model with Flow"
nav_order: 5
parent: "Module 14: Deep Learning with H20"
grand_parent: Welcome
---

# Procedure 4: Recalling a Logistic Regression model with Flow

To recall this logistic regression model from flow, navigate to:

``` r
Scores >>> Predict
```

![img.png](img.png)

The predict cell will be added to the Flow:

![img_1.png](img_1.png)

The recall of the model may assume that a new frame has been created in flow, but for this example, the validation frame will be recalled via the logistic regression, trained, model.  Firstly, set the model to recall:

![img_2.png](img_2.png)

Thereafter, select the data frame to process through the model:

![img_3.png](img_3.png)

Upon selecting the input parameters, click the predict button to complete the prediction.  A cell detailing the output will be created:

![img_4.png](img_4.png)

It is sensible at this stage to combine the predictions with the original dataset.  To combine the predictions with the original dataset, simply click the Combine Predictions with Frame button:

![img_5.png](img_5.png)

Upon combining the predictions with the original dataset, the dataset will be available for download:

![img_6.png](img_6.png)

To interact with the newly created data frame click on the View Frame button:

![img_7.png](img_7.png)

The View Frame functionality provides for the downloading and further manipulation of the data frame:

![img_8.png](img_8.png)

The process thus far uses the Flow user interface to create something akin to a script, where it is the flow tool that is sending instructions to the H2O API.  It would be far less cumbersome to use R scripting to achieve such flows.