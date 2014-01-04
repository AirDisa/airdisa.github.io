---
layout:    post
title:     Jekyll Plugins
excerpt:   Extend Jekyll with plugins.
date:      2013-12-28 09:11:36
published: true
category:  jekyll
tags:      jekyll
---

Taking your Jekyll to the next level in the most painless way probably means traversing and utilizing something that works with the [plugin architecture][jekyll-plugins]. I decided that before I roll-my-own plugin to give it a whirl with something that looks like it was sanely written. I ended up nixing a few things that looked useful but that relied on too much stuff (like external API). If anyone is going to leverage external API it is going to be my doing explicitly. Something I should probably write is a translator, or pre-processor of files that takes place before the Jekyll build process.

Before I dig in ambitious, I like to explore what is readily available and am now trying out the plugin for related\_posts that utilizes LSI (Latent Semantic Indexing). I found people like to [monkey-patch][monkey-patch] related_posts using their keywords instead. There is always classification by humans. I prefer to fully comprehend feature before dismissing them, though I admit I can run out of patience just as easily. To persevere is to come back another day to the problem. The LSI plugin defaults to a list by date, as others have found. It also depends on the gsl gem to work properly, which is something they might have missed.

[jekyll-plugins]: http://jekyllrb.com/docs/plugins/
[monkey-patch]: http://en.wikipedia.org/wiki/Monkey_patch
