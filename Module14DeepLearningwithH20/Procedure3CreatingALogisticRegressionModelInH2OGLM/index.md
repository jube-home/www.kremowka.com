---
layout: default
title: "Procedure 3: Creating a Logistic Regression model in H2O (GLM)"
nav_order: 4
parent: "Module 14: Deep Learning with H20"
grand_parent: Welcome
---

# Procedure 3: Creating a Logistic Regression model in H2O (GLM)

With the data loaded, a model now needs to be trained.  Navigate to Models to see the available algorithms:

``` r
Models
```

![img.png](img.png)

In this case, the algorithm is Generalised Linear Modelling (this is Logistic Regression).  Click this model to create the cell in flow:

![img_1.png](img_1.png)

There are a multitude of parameters that are quite outside the scope of this document, for the purposes of this document, simply specify the Training and Validation Hex sets:

![img_2.png](img_2.png)

Thereafter, specify the dependent variable, known as the Response Column in H2O:

![img_3.png](img_3.png)

In this case the Dependent Variable is titled as the same:

![img_4.png](img_4.png)

Scroll to the base of the cell and click Build Model to initiate the training process:

![img_5.png](img_5.png)

The training process will begin with progress being written out to a newly created job cell:

![img_6.png](img_6.png)

At this stage a Logistic Regression model has been created. It is a good idea to save the flow by navigating:

``` r
Flow >>> Save Flow
```

![img_7.png](img_7.png)