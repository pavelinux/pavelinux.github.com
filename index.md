---
layout: page
tagline: "SysAdmin and Programming with Python"
title: "A Cup of Python"
description: "index page"
category: Scientific Programming, sysadmin
tags: [python, bash, programming, scripting, simulations]
---
{% include JB/setup %}
**A Cup of Python** is a personal blog about some Python projects and Sysadmin
duties in GNU/Linux and UNIX.

We start this serie of posts by defining some goals, topics and categories. In this blog we:

* Develop small and simple models using programming elements and structures
based on Numerical Methods.
* This programs should give an approximation to previously defined numerical or physical problems.
* These results may be improved by iteration or redefiniton of the models.
* Also we explain some sysadmin tasks (in Linux, mainly) which are solved
for not reinveinting the wheel

Here are some recent posts for start reading A Cup of Python!
List of Posts:
<ul>
    {% for post in site.posts %}
    <li>
    <a href="{{ post.url }}">{{ post.date | date_to_string }} » {{ post.title }} </a>
    </li>
    {% endfor %} 
</ul>
Hope you enjoy them!
