---
layout:     post
title:      Front Matter by Disa Johnson @AirDisa
excerpt:    Jekyll templates their 'Front Matter' meta code.
date:       2013-12-26 10:36:55
published:  true
category:   jekyll
tags:       jekyll
---

The Jekyll templates use a plain text file interface for populating website pages dynamically, and it's got blog aware features for coders to take advantage of. The idea is simple, pretty powerful, and can leverage your programming skills fast. It dynamically translates blocks of '[Front Matter][front-matter]' code in plain text files to static code for the Web.

{% highlight YAML %}
---
layout: post
title: First Post
excerpt: I learned Jekyll in one day. You can too!
date: 2013-12-25 17:28:14
published: true
category: jekyll
tags: jekyll
---
{% endhighlight %}

People who don't code might ask why. Why code something from scratch when instead you can go with ready-made Wordpress? The answer can only lie in your love for learning code. You either have it, or you don't. There is no rational reason to take the time to learn this stuff when you can literally fire up Wordpress and write, like what writers do.

Learning to code takes perseverance, and concentration. Front matter is simple enough that it doesn't require much coding skill. It can be learned quickly to be a nice platform to get acquainted with coding. Jekyll also uses [Redcarpet][red-carpet] for markdown, which gently gets into trickier business where the dynamic power really is.

[red-carpet]: https://github.com/vmg/redcarpet
[front-matter]: http://jekyllrb.com/docs/frontmatter/
