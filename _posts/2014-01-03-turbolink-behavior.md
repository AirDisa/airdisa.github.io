---
layout:    post
title:     Turbolink Behavior
excerpt:   Behavior has me suspecting turbolink style gotchas
date:      2014-01-03 11:40:26
published: true
category:  wordpress
tags:      wordpress
---

One of the things that came built into Rails 4.0 was turbolinks. Not only was the name the butt of some developer jokes in my presence on more than one ocassion, there was plenty of complaining online with advice how to switch them off. I did not want to dismiss them too quickly. I want to understand the implications of something rather than switch it all off from experiencing some early adoption annoyances.

In my projects, for pages that are particularly laden with JavaScript, I would take the time to write links with the accompanying switch off in order to leave Turbolinks on, globally. This exercise required of me that I learn their behavior better, exactly what I wanted. I found learning Turbolinks this way paid off in recognizing these behaviors elsewhere, now noting how in the Chrome browser the behavior is most present.

When writing Wordpress themes, I like to use Chrome for surfing Wordpress task management screens. I get to see upload progress in the Chrome status bar, for example. I like Firefox for testing the frontend, and debugging computed frontend code for its terrific inspector. I like Safari for its default on the Mac operating system, where I can manage system processes and notifications. I ocassionally use Opera for inspiration.

I notice Turbolink-type bad behavior most prevalently in Chrome, and not always in a Rails project but incliding the admin screen of Wordpress. I am all for making static page components stick and only changing those bits that require alteration. People do not tend to notice things as readily as when they have stark contrasts to compare. It is only when this process breaks down, when a plain refresh will not do that people notice.
