---
layout:    post
title:     Jekyll Drawback
excerpt:   In the land of roses and honey, got a bee sting
date:      2014-01-04 19:13:58
published: false
category:  jekyll
tags:      jekyll
---

It works! There is one small caveat though that I had seen hints of before commiting all this time to learning and running Jekyll like with scissors in my hands. It is not a real deal breaker and that is why I remained confortable moving forward. The idea of hosting at GitHub means I lose control of potentially important host files. I think .htaccess is totally off limits.

The hints I saw that had me concerned (and of course I can map DNS via domain management and proxy GitHub instead of wholly host there) is 301 redirecting is going to be difficult without something additional I need. I can insert meta refresh statements with 0 for the time argument, which is treated like 301, but it is not in fact a 301. I have a page I want to 301 redirect.

What to do? I think the answer lies in writing a plugin past those I have come across which rely on meta refresh. If successful that would be good news for future Jekyll users anyhow, and I get a new open source project out of the deal. There has to be a Ruby method that invokes a 301 response code. Once again, thinking on GitHub hosting may blow up the idea altogether.
