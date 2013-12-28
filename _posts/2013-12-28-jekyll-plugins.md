---
layout:    post
title:     Jekyll Plugins
excerpt:   Extend Jekyll by hacking your plugins.
date:      2013-12-28 09:11:36
published: true
category:  jekyll
tags:      jekyll
---

Taking your Jekyll to the next level in the most painless way probably means traversing and utilizing something that works with the [plugin architecture][jekyll-plugins]. I decided that before I roll-my-own plugin to give it a whirl with something that looks like it was written sanely. I ended up nixing a few things that looked useful but that relied on too much outside stuff (like an external API).

If anyone is going to hack on my site and leverage an external API it is going to be me. Something I should probably dabble in would be to write a translator or pre-processor of my files that takes place before build, like encoding html entities so I can write with apostrophes and quotes more naturally. It is just a thought, and I also like the result writing without them.

I cringe at code that relies on other code. I have experienced problems, sometimes even upon installation and my machine(s) are all litered with a veritable Sargasso Sea of software remnants barely used or never used at all because some installation went haywire with something else on the machine and had to be aborted. Developers do this stuff with their environment and I like mine stripped bare.

I will dabble in one whose only requirement is a Gem that I already know: Nokogiri.

[jekyll-plugins]: http://jekyllrb.com/docs/plugins/
