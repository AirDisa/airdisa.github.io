---
layout:     post
title:      Front Matter
excerpt:    Jekyll templates their 'Front Matter' meta code.
date:       2013-12-26 10:36:55
published:  false
category:   jekyll
tags:       jekyll
---

The Jekyll templates use a plain text file interface for populating website pages dynamically, and it's got blog aware features for coders to take advantage of. The idea is pretty simple, powerful, and can leverage your programming know-how fast. It dynamically translates '[Front Matter][front-matter]' blocks from plain text files into static HTML for the Web.

People who don't code might ask why. Why code something from scratch like this instead of going with something ready-made like Wordpress? The answer can only lie with the love for learning code. There is no rational reason to take the time when you can literally fire up Wordpress and write content without coding a thing. That's what writers should do.

Learning to code takes perseverance and concentration. Front matter is simple enough that Jekyll really doesn't require much coding skill, so it can be learned quick or be the perfect platform to learn in order to get into coding without diving headfirst into Java. Java is an awesome language and Jekyll doesn't compare. Jekyll can get you started more easily.

{% highlight YAML &}
---
layout: default
title: First Post
excerpt: I learned Jekyll in one day. You can too!
date: 2013-12-25 17:28:14
published: false
category: jekyll
tags: jekyll
---
{% endhighlight %}

[front-matter]: http://jekyllrb.com/docs/frontmatter/
