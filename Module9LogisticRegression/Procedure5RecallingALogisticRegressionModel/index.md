---
layout: default
title: "Procedure 5: Recalling a Logistic Regression Model"
nav_order: 6
parent: "Module 9: Logistic Regression"
grand_parent: Welcome
---

# Procedure 5: Recalling a Logistic Regression Model

It is fairly self-explanatory to deploy a logistic model, recall is performed in the same manner as a linear regression model.  As with the lm() product, the glm() model has a predict.gml() function to create a prediction for all values in a data frame.  The signature bears stark resemblance to that of the predict.lm() function:

``` r
AutomaticLogisticRegression <- predict.glm(LogisticRegressionModel,FraudRisk)
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

It can be seen that a new vector has been created in the environment pane which will contain the predictions for each entry in the FraudRisk Data Frame:

![img_2.png](img_2.png)

For completeness, merge the newly created vector into the FraudRisk data frame:

``` r
FraudRisk <- mutate(FraudRisk, AutomaticLogisticRegression)
```

![img_3.png](img_3.png)

Run the line of script to console:

![img_4.png](img_4.png)