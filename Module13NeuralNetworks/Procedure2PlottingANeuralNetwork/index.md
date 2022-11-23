---
layout: default
title: "Procedure 2: Plotting a Neural Network"
nav_order: 3
parent: "Module 13: Neural Networks"
grand_parent: Welcome
---

# Procedure 2: Plotting a Neural Network

It is often stated that a neural network is an unexplainable modelling techniques, which practically holds some truth, but to those with a background in regression modelling, explaining the model is not insurmountable.

The neuralnet object that was created allows for the plotting of the neural network using the base plot() function.  Simply call plot() passing the neural network object as an argument:

``` r
plot(NeuralNetworkFourByOne)
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

A plot is created of the neural network bearing stark resemblance to conceptual models put forward in this training manual,  and in a model of less complexity, is in fact explainable and quite reproducible on a manual basis:

![img_2.png](img_2.png)

As the model becomes more and more complex,  with the addition of more and more features, layers and processing elements, the neural network will naturally become less and less explainable.