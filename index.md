---
layout: page
title: "Programming with Python"
tagline: A Cup of Python in the Morning!
description: "index page"
category: Scientific Programming
tags: [python, programming, simulations]
---
{% include JB/setup %}
**A Cup of Python in the morning** is a personal page about some little Python projects which are supposed to be read while you 
enjoy a *delicious cup of coffee*. 

##The goals

We start this serie of posts by defining our purposes:

* To develop small and simple models using programming elements and structures based on Numerical Methods class notes to write Python programs. 
* This programs should give an approximation to previously defined numerical or physical problems.
* These results may be improved by iteration or redefiniton of the models.

###Here we include some little programs to start a Cup of Python!
List of Python Programs:

    {% for post in site.posts %}
        {{ post.date | date_to_string }} » {{ site.posts }}
    {% endfor %} 

Hope you enjoy them!
