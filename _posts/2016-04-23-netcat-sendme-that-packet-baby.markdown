---
layout: post
title: Netcat. Send me that packet baby
date: 2016-04-23 17:40
categories: UNIX linux sysadmin
---
Netcat is famous for being one of the most versatile and complete UNIX
tool. It is considered a six blade knife of TCP/IP/UDP ([do anything for
you](https://youtu.be/wADwIZ6V3NY) ;-)

**First act**:
In the box (mine is called *escarabajo*) where we want to get the files backed
up, we open the port
where the transfer will take place. Also it is a good idea (if the transfer
will be large )to compress and
extract the files to be sent *on the fly*. So, in this step we prepare the set:
{% highlight shell %}
nc -l 7721 | tar xvzf -
{% endhighlight %}

**Second act**:
In the server where we want to send the directories to back up, we simply put
us in front of the directories and start the transfer:
{% highlight shell %}
tar -czf - * | nc escarabajo 7721
{% endhighlight %}
