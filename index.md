---
layout: page
title: "Programming with Python"
tagline: "A Cup of Python"
description: "index page"
category: Scientific Programming
tags: [python, programming, simulations]
---
{% include JB/setup %}
**A Cup of Python** is a personal blog about some little Python projects which are supposed to be read while you enjoy a *delicious cup of coffee*. 

##The goals

We start this serie of posts by defining our purposes:

* To develop small and simple models using programming elements and structures based on Numerical Methods class notes to write Python programs. 
* This programs should give an approximation to previously defined numerical or physical problems.
* These results may be improved by iteration or redefiniton of the models.

###Here are some recent posts for start reading A Cup of Python!
List of Posts:
    {% for post in site.posts %}
    {{site.production_url}}{{ post.url }}
    {{ post.date | date_to_string }} » {{ post.title }} {{post.url}}
    {% endfor %} 
Hope you enjoy them!
