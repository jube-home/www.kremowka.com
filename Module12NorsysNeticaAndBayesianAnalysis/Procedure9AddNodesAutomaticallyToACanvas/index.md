---
layout: default
title: "Procedure 9: Add Nodes Automatically to a Canvas"
nav_order: 10
parent: "Module 12: Norsys Netica and Bayesian Analysis"
grand_parent: Welcome
---

# Procedure 9: Add Nodes Automatically to a Canvas

The process of manually adding nodes to a canvas is quite laborious and with a key benefit of Bayesian networks being the ability to handle extremely large networks with hundreds of nodes, impractical.  Furthermore, Bayesian techniques are inherently state based, which would rely on a process of dividing continuous variables into appropriate state bins. 

Netica has the ability to infer columns from a file, thus allowing for automation in the creation of nodes on the canvas.

Start by creating a blank canvas as demonstrated:

![img.png](img.png)

To infer and then add the case file nodes, click Cases in the menu Item, then click or hover on the Learn sub menu item, then click Add Case File Nodes:

![img_1.png](img_1.png)

When the dialog box opens, select the file CreditRisk.csv:

![img_2.png](img_2.png)

Clicking Open will begin the process of creating nodes based upon the Variables name coupled with an analysis of the number of states within that Variable.  In the event that a variable is determined to be continuous, a prompt will be displayed to determine the number of states to set for this variable:

![img_3.png](img_3.png)

Specify the number of states deemed appropriate for the variable, then click ok.  Repeat for each variable until all of the nodes have been added to the canvas:

![img_4.png](img_4.png)