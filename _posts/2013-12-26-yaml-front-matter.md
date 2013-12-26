---
layout:     post
title:      Front Matter
excerpt:    Jekyll templates their &#39;Front Matter&#39; meta code.
date:       2013-12-26 10:36:55
published:  true
category:   jekyll
tags:       jekyll
---

The Jekyll templates use a plain text file interface for populating website pages dynamically, and it&#39;s got blog aware features for coders to take advantage of. The idea is simple, pretty powerful, and can leverage your programming skills fast. It dynamically translates blocks of &#39;[Front Matter][front-matter]&#39; code in plain text files to static code for the Web.

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

People who don&#39;t code might ask why. Why code something from scratch when instead you can go with ready-made Wordpress? The answer can only lie in your love for learning code. You either love it, or you don&#39;t. There is no rational reason to take the time to learn this stuff when you can literally fire up Wordpress and write, like what writers do.

Learning to code takes perseverance, and concentration. Front matter is simple enough that it doesn&#39;t require much coding skill to start. It can be learned quickly enough to serve as a nice platform for getting acquainted with coding. Jekyll also uses [Redcarpet][red-carpet] for markdown, which gently gets into trickier business (where the dynamic power really is). Check it out!

[red-carpet]: https://github.com/vmg/redcarpet
[front-matter]: http://jekyllrb.com/docs/frontmatter/
