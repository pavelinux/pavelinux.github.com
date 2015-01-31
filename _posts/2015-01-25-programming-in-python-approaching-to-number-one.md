---
layout: post
title: "Programming in Python: Approaching to number One"
description: "The use  "
categories: [Programming, Python, Series] 
tags: [cycles, while, series, convergence]
---
{% include JB/setup %}
Here we use one of the control structures most used on every programming language. We are talking about 
the *while* cycle statement which is used for iteration problems.
In this post we use the cycle 
for calculating a *sum* of the form:
$\displaystyle\sum_{k = 1}^{n} \frac{1}{2^{k}}= 1$



>#!/usr/bin/env python
># This program computes a serie of the type
># 1 =  1 / 2 ** 1 + ... + 1 / ( 2 ** n )
># and compares the given value to the calculated
>
>print "This program calculates the number of terms needed to get a desired approach to 1.0 using the expression"
>print "1 = 1 / 2 ** 1 + ... + 1 / ( 2 ** n )"
>print "It is considered a good value 0.990."
>print "Write down the tolerance desired. (For instance: tol = 0.01)"
>
>value = 1.000
>tol = float(raw_input(' tol -> '))
>output = 0.000
>i = 1
>desv = 1.000
>
>while desv >= tol:
>    output = output + (1.00 / (2 ** i)) 
>    i += 1
>    desv = abs(value - output)
>    print "1.0000 -", output, " = ", desv
>
>print "You get: ", output, " with: ", i - 1, " terms"