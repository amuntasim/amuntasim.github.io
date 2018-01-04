---
layout: post
title:  Liquid using or in views
date:   2015-01-04 11:40:16
description:   
---
There is a logical 'or' operator in liquid  but if you want to display something conditional, that might not be helpful.

If want to display second value if the first value is not there for example "page.title or page.date", we would need something like this



{% highlight js %}
	page.title | default: page.date
{% endhighlight %}

Tested in Jekyll Liquid

