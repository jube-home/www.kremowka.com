---
layout: default
title: "Procedure 4: Enter subjective probabilities for each consequence"
nav_order: 5
parent: "Module 12: Norsys Netica and Bayesian Analysis"
grand_parent: Welcome
---

# Procedure 4: Enter subjective probabilities for each consequence

In creating a consequence, with many potential causes, and with the causes being state based (which in this example is Yes \ No), a finite set of scenarios that cause a consequence can now be inferred by Netica.

To view the finite scenarios that can cause a consequence, right click on the consequence node, in this case Default, the click Table (short for Node \ Conditional Probability Table):

![img.png](img.png)

The node probability infers every possible scenario in the Bayesian Network, calling for subjective probabilities to be included:

![img_1.png](img_1.png)

In this simple example, there are two scenarios which require subjective probabilities, however, with more nodes this GREATLY expands.  Subjective probability needs to be apportioned to each scenario, rather belief (hence Bayesian Belief Networks).

In this example apportion the following subjective probability:

* If Count Bank Card Products > 3 then P(Default) = 9%
* If NOT Count Bank Card Products > 3 then P(Default) = 3%

These probabilities would be updated in the corresponding table:

![img_2.png](img_2.png)

Clicking on the Fill Missing Probabilities Icon will complete the missing probabilities where possible, summing to 100%:

![img_3.png](img_3.png)

![img_4.png](img_4.png)

Click Apply, then Ok to close the window. The node probabilities have been set, however the network has not been compiled, and so the states retain the default probabilities:

![img_5.png](img_5.png)

To compile the network, click on the lightning bolt icon in the menu to compile the network and set the probabilities:

![img_6.png](img_6.png)

![img_7.png](img_7.png)

The Bayesian network has now been compiled and is ready to both predict Default and explain Default via Bayesian Inference.