---
layout: post
title: Forwarding a "hidden" port
date: 2016-04-25 13:00
categories: UNIX linux sysadmin ssh
comments: true
---
Sometimes, when we are at home doing some work (for example, some HTML) behind  *the office firewalled* unix web server and the box 
has the 80 port closed to internet, 
it is useful to *foward* the 80 active protected port to our home network. In order to do that there are
two possible solutions, depending the OS we are using: 

The first one, if we are working on a unix box, is directly forward the 80 port, using a *whateveryoulike*
port. For example:
{% highlight shell %}
ssh -L 7721:localhost:80 user@mydomain.com 
{% endhighlight %}
In this command, the first part, we are forwarding the *hidden 80* port to our *whateverwelike* localhost 7721 port.
The rest of the command: We are logging to the unix web server through *22* port (or the port you are using to connect through ssh).

Now you can check the result using, for example *netstat* or *ss*:
{% highlight shell %}
# ss -tnlp |less
tcp        0      0 127.0.0.1:7721          0.0.0.0:*               LISTEN    24319/ssh
{% endhighlight %}

Then, fire up your web browser and write your forwarded url [http://localhost:7721](http://localhost:7721)

The other possible solution, if you are working on a windows machine, is to use [Putty](http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html).
Check this [youtube video](https://youtu.be/lxurpEIr02A)
