---
layout: default
title: "Module 14: Deep Learning with H20"
nav_order: 14
has_children: true
parent: Welcome
---

# Module 14 Deep Learning with H20

H20 is an external server-based software application that presents a variety of machine learning algorithms.  The machine learning algorithms available do not materially differ from those already presented and freely available in R.  H20 provides several useful features for deep learning though:

* Compression of data while processing, in a hex format.  This makes the memory requirements less burdensome, keeping in mind that R keeps data frames in memory otherwise and;
* Compatibility with a GPU to facilitate Deep Neural Networks and Deep Learning.

* H20 has exceptionally well coupled with R, and while processing will take place in the H20 server, it is as though it is taking place within RStudio.  H20 exists in the mix of tools predominately because of its ability to use a GPU for deep learning as well as providing granular control over cross validation and activation functions.

* H20 is fundamentally an API led platform and R is just one tool that can make use of the tool via API.  H20 has its own tool, called Flow, that can invoke these API's and make for a self-service user interface, setting a low bar to create models.  These procedures will use Flow to create a familiarity with H20, before seeking to replicate the processes with R commands, which is how most users will tend to interact with H20.