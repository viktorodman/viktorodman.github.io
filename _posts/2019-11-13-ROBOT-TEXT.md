---
layout: post
title: Robots.txt
img: /assets/roboto.png/
permalink: /posts/robots-text/
comments: true
---

# What is robots.txt and how have you configure it for your site?

Robots.txt is a text document used to communicate with "Web Robots" that search the web.
The robots.txt document tells the web robots what information they are allowed to access on the website.

I've configured my robot.txt to not allow any information to accessed by web robots.

###### My robots.txt

{% highlight Plain Text %}
User-agents: *
Disallow: /
{% endhighlight %}