---
layout: default
title: "Module 15: Monte Carlo Model Simulation"
nav_order: 15
has_children: true
parent: Welcome
---

# Module 16: Monte Carlo Model Simulation

In this example, the result is the simulation of the neural network model that was created in H2O.  It follows that we need to create a dataframe with the same specification the training data set.

For the purposes of our example, we are going to create triangular distributions comprised of the Minimum Value, the Maximum Value and the Mean.  This simulated dataframe will be 100,000 records in length.

This procedure will focus on creating this vector for a single variable, before providing a block of script to achieve this for each variable at the end of the procedure.

Firstly, install the triangle package:

![img.png](img.png)

Load the library:

library(triangle)

![img_1.png](img_1.png)

Run the line of script to console:

![img_2.png](img_2.png)