---
layout:    post
title:     Jekyll Drawback
excerpt:   In the land of roses and honey, a sting
date:      2014-01-02 09:28:18
published: true
category:  jekyll
tags:      jekyll
---

It works! There is one caveat. I had seen hints of this before committing my time to learning and running Jekyll, like with scissors in my hands and it not a deal breaker. It is merely a complication which is why I remained comfortable moving forward. I am hoping I can implement one of a few workarounds milling about my brain. Hosting at GitHub means I lose control over important host files. The [Jekyll plugin warning][warning] states that GitHub runs Jekyll with the --safe option, effectively disabling any runtime plugins from executing. This is a perfectly suitable measure for security at GitHub.

We must make sure our files deliver what we intend as purely static files. Static sites are at least faster, no question. Options I miss are available when .htaccess directives are adhered to, which are definitely off-limits at GitHub. These restrictions had me wondering about applying 301 server-response codes to move pages, code that both updates user bookmarks and search engine listings. No such early luck, what to do? I can always develop [architecture][architecture] that writes meta refresh into static HTML. Then there is this thread about a plugin [white-list][merged] which looks promising. I may host anyway and proxy GitHub for flat files.

[warning]: http://jekyllrb.com/docs/plugins/
[architecture]: http://pixelcog.com/blog/2013/jekyll-from-scratch-core-architecture/
[merged]: https://github.com/jekyll/jekyll/pull/1657
