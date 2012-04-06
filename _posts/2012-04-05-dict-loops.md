---
layout: post
title: Dictionary assignment in a loop
---

You can assign to any expression in a loop:

{% highlight python %}
l = [(1, 2), (3, 4), (5, 6)]
d = {}
for d['a'], d['b'] in l:
    print d
{% endhighlight %}
