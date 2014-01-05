---
layout:     post
title:      Front Matter
excerpt:    I learned Jekyll in one day. You can too!
date:       2013-12-26 10:36:55
published:  true
category:   jekyll
tags:       jekyll
---

The Jekyll templates use a plain text file interface for populating website pages dynamically, and it is got blog aware features for coders to take advantage of. The idea is powerful and simple enough to leverage virtually any programming skills fast. If you know Ruby you can take it a lot further. Jekyll dynamically translates blocks of plain text &#39;[Front Matter][front-matter]&#39; to static files. People who do not code might ask why. Why code something from scratch when instead you can go with ready-made Wordpress?

{% highlight yaml %}
---
layout: post
title: Front Matter
excerpt: I learned Jekyll in one day. You can too!
date: 2013-12-25 17:28:14
published: true
category: jekyll
tags: jekyll
---
{% endhighlight %}

The answer can only lie in your love for learning code. You either love it, or not. There is no good reason and only that rationality to take the time to learn this stuff when you can literally fire up Wordpress and write, like what writers do. Learning to code takes perseverance and concentration. Front matter is simple enough that it can serve for getting acquainted with further coding. Jekyll uses [Redcarpet][red-carpet] for markdown which gently gets into trickier business (where the dynamic power really is). Check it out!

[front-matter]: http://jekyllrb.com/docs/frontmatter/
[red-carpet]: https://github.com/vmg/redcarpet
