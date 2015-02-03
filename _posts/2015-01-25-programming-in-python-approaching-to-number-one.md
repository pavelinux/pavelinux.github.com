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

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;}
.tg .tg-hgcj{font-weight:bold;text-align:center}
.tg .tg-s6z2{text-align:center}
</style>
<table class="tg">
  <tr>
    <th class="tg-hgcj">Steps</th>
    <th class="tg-hgcj">Output</th>
    <th class="tg-hgcj">Tol.</th>
  </tr>
  <tr>
    <td class="tg-s6z2">1</td>
    <td class="tg-s6z2">0.5</td>
    <td class="tg-s6z2">0.5</td>
  </tr>
  <tr>
    <td class="tg-s6z2">2</td>
    <td class="tg-s6z2">0.75</td>
    <td class="tg-s6z2">0.25</td>
  </tr>
  <tr>
    <td class="tg-s6z2">3</td>
    <td class="tg-s6z2">0.875</td>
    <td class="tg-s6z2">0.125</td>
  </tr>
  <tr>
    <td class="tg-s6z2">4</td>
    <td class="tg-s6z2">0.9375</td>
    <td class="tg-s6z2">0.0625</td>
  </tr>
  <tr>
    <td class="tg-s6z2">5</td>
    <td class="tg-s6z2">0.96875</td>
    <td class="tg-s6z2">0.03125</td>
  </tr>
  <tr>
    <td class="tg-s6z2">6</td>
    <td class="tg-s6z2">0.984375</td>
    <td class="tg-s6z2">0.015625</td>
  </tr>
  <tr>
    <td class="tg-s6z2">7</td>
    <td class="tg-s6z2">0.9921875</td>
    <td class="tg-s6z2">0.0078125</td>
  </tr>
</table>

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
