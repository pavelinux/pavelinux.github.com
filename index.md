---
layout: page
title: "Programming with Python"
tagline: A Cup of Python in the Morning!
description: "index page"
category: Scientific Programming
tags: [python, programming, simulations]
---
{% include JB/setup %}
##The goals

We start this serie of posts by defining our purposes:

* To develop small and simple models using programming elements and structures based on Numerical Methods notes to develop Python programs. 
* This programs should give an approximation to previously defined physical problems.
* These results may be improved by iteration or redefiniton of the models.

#Here we include some little programs to start a Cup of Python!
Python Programs:

    {% for post in site.posts %}
    {{ post.date | date_to_string }} » {{ post.title }}
    {% endfor %} 
