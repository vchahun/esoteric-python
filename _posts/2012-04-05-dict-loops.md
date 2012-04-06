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

    {'a': 1, 'b': 2}
    {'a': 3, 'b': 4}
    {'a': 5, 'b': 6}

Equivalent evil version:

{% highlight python %}
l = [(1, 2), (3, 4), (5, 6)]

magic = (({}, a, b) for (a, b) in l)
for d, d['a'], d['b'] in magic:
    print d
{% endhighlight %}
