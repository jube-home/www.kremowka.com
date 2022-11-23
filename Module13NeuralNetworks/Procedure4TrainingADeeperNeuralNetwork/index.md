---
layout: default
title: "Procedure 4: Training a Deeper Neural Network"
nav_order: 5
parent: "Module 13: Neural Networks"
grand_parent: Welcome
---

# Procedure 4: Training a Deeper Neural Network

A neural network was trained having only a single hidden layer, albeit with several processing elements.  Deep learning is the notion of having many more hidden layers and generally many more processing elements.  Each layer is able to achieve abstraction autonomously, finding patterns that may not be apparent in manual abstraction.  HOWEVER, it is lazy, adds valuable computational expense in recall (which begins to matter in super high throughput environments), as such deep learning can have circumvented to an extent, given more creativity in the abstraction phase.

In this example, a much deeper neural network will be created where the same ten inputs will be used.  The first hidden layer will have 8 processing elements, the second hidden layer will have 6 processing elements, the third hidden layer will have 4 processing elements yielding an output.

A single value specifying just the number of processing elements was provided, where it was inferred that only a single hidden later is applicable.  In this procedure, it is necessary to construct a vector, with each vector entry corresponding to a hidden layer, with the value of that hidden layer entry being the processing elements for that hidden layer:

``` r
NueralNetworkDeep <- NeuralNetworkFourByOne <- neuralnet(Dependent ~ Skew_3 + Max_4 + PointStep_16 + Close_3 + Close_4 + PointStep_17_ZScore + PointStep_15 + TypicalValue_4 + Range_4 + Range_2, data = FDX, hidden = c(8,6,4))
```

![img.png](img.png)

Run the line of script to console, expect it to take some time:

![img_1.png](img_1.png)

Plot the function to inspect the neural network:

``` r
plot(NueralNetworkDeep)
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

The plot has dramatically increased in complexity. It can be observed that the Neural Network now has three hidden layers, the first having 8 processing elements, the second having 6 processing elements and the third having 4 processing elements:

![img_4.png](img_4.png)

Naturally, this complexity is only worthwhile in the event that the classification accuracy has improved.  As such, invoke compute and extract the results:

``` r
ComputedModelDeep <- compute(NueralNetworkDeep,FDX[,c("Skew_3","Max_4","PointStep_16","Close_3","Close_4","PointStep_17_ZScore","PointStep_15","TypicalValue_4","Range_4","Range_2")])
```

![img_5.png](img_5.png)

Run the line of script to console:

![img_6.png](img_6.png)

Extract the predictions to a list, for conversion to a vector later:

``` r
FDXPredeictionsDeep <- ComputedModelDeep$net.result
```

![img_7.png](img_7.png)

Run the line of script to console:

Appraise the correlations between the predictions and the dependent variable:

``` r
cor(FDXPredeictionsDeep,FDX$Dependent, use="complete",method="pearson")
```

![img_8.png](img_8.png)

Run the line of script to console:

![img_9.png](img_9.png)

It can be seen that the correlation between predicted and actual has leaped to a staggering 0.91 in response to increasing the complexity of the model. 