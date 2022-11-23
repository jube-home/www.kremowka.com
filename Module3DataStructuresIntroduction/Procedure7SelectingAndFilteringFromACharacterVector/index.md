---
layout: default
title: "Procedure 7: Selecting and Filtering from a Character Vector"
nav_order: 8
parent: "Module 3: Data Structures Introduction"
grand_parent: Welcome
---

# Procedure 7: Selecting and Filtering from a Character Vector

Once a Vector has been named,  attaching a label to each value,  it can be selected using the [] square bracket structure.  In this example,  the age for Tom needs to be extracted by typing:

``` r
Ages["Tom"]
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

Tom’s age is returned as 22, rather the value in the Vector carrying the label "Tom" is returned as 22.  

To select more than one label, it is a matter of creating a Vector with the criteria then passing that Vector inside the [] square brackets.  In this example, selecting Tom and Dick:

``` r
Ages[c("Tom","Dick")]
```

![img_2.png](img_2.png)

Run the line of script to console:

![img_3.png](img_3.png)