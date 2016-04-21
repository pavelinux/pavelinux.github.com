---
layout: post
title: Copying dirs and files fastly 
date: 2016-04-21 18:06:42 
categories: UNIX linux sysadmin
---
Sometimes we need to backup some big directories in a UNIX box. 

For example if we would like to copy the home directory to a USB device, just
use *cpio*, *find* and that's it:
{% highlight shell %}

find /home -print0 -depth | cpio --null -pvd /media/username/backups

{% endhighlight %}
Check out the tutorial in [GNU-cpio]

[GNU-cpio]: https://www.gnu.org/software/cpio/manual/html_node/index.html
