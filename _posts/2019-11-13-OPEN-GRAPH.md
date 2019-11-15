---
layout: post
title: Open Graph
img: /pics/open-graph-logo.png/
permalink: /posts/open-graph/
comments: true
---

# What is Open Graph and how do you make use of it?

Open Graph is used to create graph objects that can be used to represent the webpage when its shared on different social media websites. The graph object is created by using the provided metadata on the website. 

I've added meta tags in the head element of my webpages.


{% highlight HTML %}
<meta property="og:title" content="{'{ page.title }'}" />
<meta property="og:type" content="website" />
<meta property="og:url" content="{'{ page.permalink }'}" />
<meta property="og:image" content="{'{ site.open-graph-img }'}" />
{% endhighlight %}