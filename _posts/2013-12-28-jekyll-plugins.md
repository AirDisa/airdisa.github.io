---
layout:    post
title:     Jekyll Plugins
excerpt:   Extend Jekyll by hacking plugins.
date:      2013-12-28 09:11:36
published: true
category:  jekyll
tags:      jekyll
---

Taking your Jekyll to the next level in the most painless way probably means traversing and utilizing something that works with the [plugin architecture][jekyll-plugins]. I decided that before I roll-my-own plugin to give it a whirl with something that looks like it was sanely written. I ended up nixing a few things that looked useful but that relied on too much stuff (like external API).

If anyone is going to leverage external API it is going to be my choosing. Something I should probably write is a translator or pre-processor of files that takes place before Jekyll build, like encoding html entities so I can write with apostrophes and quotes more naturally. It is just an idea and I like the effect writing without them, naturally.

I might look into a plugin where the only requirement is a Gem I already know: Nokogiri. I cringe thinking on code that relies on other code I might not know. I picture littered machines as though they are a Sargasso Sea of software, remnants of bits barely used or never used at all. Some installations go haywire and have to be aborted. It wastes so much time I like a machine stripped bare.

[jekyll-plugins]: http://jekyllrb.com/docs/plugins/
