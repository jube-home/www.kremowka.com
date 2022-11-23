---
layout: default
title: "Procedure 3: Searching with Regular Expressions"
nav_order: 4
parent: "Module 4: Loading, Shaping and Merging Data"
grand_parent: Welcome
---

# Procedure 3: Searching with Regular Expressions

Beforehand the substr() function was used to search for any occurrence of the string "Richard".  The substr() is a very limited function and assumes a certain amount of structure exists in the base string.  The grepl() function allows for the searching of a character string with regular expressions rather than specific location based arguments.  Regular Expressions are a sequence of symbols and characters expressing a string, or pattern, describing a search within a longer piece of text.  Regular Expressions can be quite complex but they are extraordinarily powerful for string matching.

This procedure sets out to replicate the substr() function using Regular Expressions and the grepl() function,  searching for any string that starts with "Richard" using the ^ symbol:

``` r
NamesGrepl <- grepl(^Richard,NamesSubstr)
```

![img.png](img.png)

Run the line of script to console:

![img_1.png](img_1.png)

Write the NamesGrepl vector out to console by typing:

``` r
NamesGrepl
```

![img_2.png](img_2.png)

It can be observed that any name string starting with "Richard" has been returned as a logical vector.  To make this abstraction useful for machine learning it is a simple matter of transforming it to a numeric vector by typing:

``` r
NameGreplNumeric <- as.numeric(NamesGrepl)
```

![img_3.png](img_3.png)

Run the line of script to console:

![img_4.png](img_4.png)

Write out the NamesGrepNumeric vector by typing:

``` r
NamesGrepNumeric
```

![img_5.png](img_5.png)

Run the line of script to console:

![img_6.png](img_6.png)

It can be seen that this vector is now more appropriate for machine learning.  Nesting the functions,  the procedure could be created more succinctly by typing:

``` r
NamesGrepNumericNested <- as.numeric(grepl("^Richard",Names))
```

![img_7.png](img_7.png)