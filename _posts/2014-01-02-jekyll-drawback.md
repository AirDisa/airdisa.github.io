---
layout:    post
title:     Jekyll Drawback
excerpt:   In the land of roses and honey, a sting
date:      2014-01-02 09:28:18
published: true
category:  jekyll
tags:      jekyll
---

It works! There is one small caveat that I had seen hints of before committing all this time to learning and running Jekyll, like with scissors in my hands. The issue is not a deal breaker, merely a complication. That is why I remained comfortable moving forward. I am hoping I can think of a workaround. Hosting at GitHub means I lose control over important host files, settings and processes.

The [Jekyll plugin warning][warning] I came across states that GitHub runs Jekyll with the --safe option, effectively disabling any runtime plugins from executing. This is a perfectly suitable measure for security at GitHub, leaving the rest of us to scramble and think of something to make sure our files are static. Static sites are nice and fast and entirely static (except for JavaScript).

Host files for options such as available with .htaccess, are off-limits at GitHub. These restrictions had me wondering about redirecting, hoping for access to 301 server-response codes. These response codes are able to perform updating both user bookmarks and search engine listings. Other solutions exist though second-rate, such as that of using 0 time argument in meta refresh using HTML.

What to do? There is always developing [architecture][architecture] that writes meta refresh, and other important files, into your static HTML. Plugins for meta refresh already exist and the thing to watch is this recent discussion about a [white-list][merged] of plugins. I have not yet fully absorbed all that is in this thread but it looks promising, definitely worth exploring and watching.

[warning]: http://jekyllrb.com/docs/plugins/
[architecture]: http://pixelcog.com/blog/2013/jekyll-from-scratch-core-architecture/
[merged]: https://github.com/jekyll/jekyll/pull/1657
