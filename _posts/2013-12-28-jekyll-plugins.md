---
layout:    post
title:     Jekyll Plugins
excerpt:   Extend Jekyll by hacking your plugins.
date:      2013-12-27 00:06:05
published: false
category:  jekyll
tags:      jekyll
---

The next thing that can take your Jekyll to the next level is utilizing the [plugin architecture][jekyll-plugins] to roll-your-own extensions with Ruby. GitHub runs them in safe mode so the idea needs to be one you can parse into the static files on your machine first. The static files will be used to power your GitHub site if that is where it is to be published.

Plugins are still perfectly suitable for certain tasks. One thought which springs to mind, is using the notion of capturing an &#39;authored on&#39; and &#39;last modified&#39; timestamp set for notifying readers with a little extra meta data. The timestamps can then also make their way into Open Graph, which has meta data containers for these data. The other neat idea which springs to mind is to wire keyworss to a search result page which can actually ve statically driven.

[jekyll-plugins]: http://jekyllrb.com/docs/plugins/
