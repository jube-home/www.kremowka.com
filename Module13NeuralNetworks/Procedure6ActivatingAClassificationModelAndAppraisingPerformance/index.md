---
layout: default
title: Procedure 6 Activating a Classification Model and Appraising Performance
nav_order: 7
parent: Module 13 Neural Networks
grand_parent: Welcome
---

# Procedure 6 Activating a Classification Model and Appraising Performance

To recall the neural network, return a value between 0 and 1 depending on the likelihood that the record is fraudulent:

``` r
FraudRiskPredictions <- FraudRiskNeuralNetwork$net.result
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

Peeking the results with the head() function:

``` r
head(FraudRiskPredictions)
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)

It can be seen that numeric values, between 0 and 1, have been returned.  The closer to one, the more likely that the record is fraudulent.   To assert a proper classification, so that a confusion matrix may be plotted to appraise performance of the model, create a vector contains a 1 where the value of FraudRiskPredictions > 0.5, else 0, yet wrapping FraudRiskPrediction with the unlist() function to transform the list output to a vector:

``` r
IsFraud <- ifelse(unlist(FraudRiskPredictions) > 0.5,1,0)
```

![img_4.png](img_4.png)

Run the line of script to console:

![img_5.png](img_5.png)

As has become customary, use a confusion matrix to appraise the value of the classifier:

``` r
library("gmodels")
CrossTable(FraudRisk$Dependent, IsFraud)
```

![img_6.png](img_6.png)

Run the block of script to console:

![img_7.png](img_7.png)

In this example, it can be seen that 720 records were classified as being fraudulent correctly.  In total, it can be seen that 901 records were classified, so the accuracy rate on predicting fraud is 79.9%, a substantial uplift on the logistic regression models created in procedure 93.  It is well worth mentioning, that for classification problems, less is very often more and rather than increase network complexity by adding more and more hidden layers and processing elements, it is often more efficient to create many more abstracted variables backed by intuitive judgement and domain expertise.