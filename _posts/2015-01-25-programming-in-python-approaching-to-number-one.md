---
layout: post
title: "Programming in Python: Approaching to number One"
description: "The use  "
categories: [Programming, Python, Series] 
tags: [cycles, while, series, convergence]
---

**H**ere we use one of the control structures most used on every
programming language. We are talking about the *while* statement which
is used for iteration problems. We use this statement for
calculating a *sum* of the form:
<center>
$$\displaystyle\sum_{k = 1}^{n} \frac{1}{2^{k}}= 1$$ 
</center>

Doing this task require to 
use an *iteration* (repeating identical or similar tasks until a condition is satisfied).

Iterations and controlled loops
===============================

The *while* cycle on Python
---------------------------

-   First item in a list

-   Second item in a list

-   Third item in a list

Some code
---------
The syntax of a *while* statement is very simple but strict on Python.

    1.  One always have to include a condition, yielding a *True* or
    *False*.

    2.  If the condition is *False* exit the *while* statement and continue
    with the rest of the statements of the program.

    3.  If the condition is *True* execute the body of the *while* cycle and
    then go back to step 1.

<pre><code>#(Previously initialize the included variables)
while desv = tol:
    output = output + (1.00 / (2 ** i)) 
    i += 1             
    desv = abs(value - output)
    print "1.0000 -", output, " = ", desv
#Note the level of indentation
#inside the statement.</code></pre>

Results
=======

Tolerance (condition for the iterarion) d = 0.01
<center>
<table>
  <tr>
    <th>Steps</th>
    <th>Output</th>
    <th>Tol.</th>
  </tr>
  <tr>
    <td>1</td>
    <td>0.5</td>
    <td>0.5</td>
  </tr>
  <tr>
    <td>2</td>
    <td>0.75</td>
    <td>0.25</td>
  </tr>
  <tr>
    <td>3</td>
    <td>0.875</td>
    <td>0.125</td>
  </tr>
  <tr>
    <td>4</td>
    <td>0.9375</td>
    <td>0.0625</td>
  </tr>
  <tr>
    <td>5</td>
    <td>0.96875</td>
    <td>0.03125</td>
  </tr>
  <tr>
    <td>6</td>
    <td>0.984375</td>
    <td>0.015625</td>
  </tr>
  <tr>
    <td>7</td>
    <td>0.9921875</td>
    <td>0.0078125</td>
  </tr>
</table>
</center>

Discussion
==========

First

Last
   This is the last item

References:
==========

1. Salas, S. L., Hille, E and Etgen, G. (2007). Calculus , 575–579.

2. Downey, Allen (2013). Think Python. How to think like a Computer
Scientist , 64–65.
- - -
