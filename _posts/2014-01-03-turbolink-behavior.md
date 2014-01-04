---
layout:    post
title:     Turbolink Behavior
excerpt:   Behavior has me suspecting turbolink gotchas.
date:      2014-01-03 11:40:26
published: true
category:  wordpress
tags:      wordpress
---

One of the things that came built into Rails 4.0 was turbolinks. Not only was the name a butt of jokes by developers in my presence, there was also plenty of complaining online with advice for how to switch them totally off. I did not want to dismiss them too quickly. I want to understand the implications of a new feature rather than switch it all off after experiencing some early adoption annoyances. There are definite turbolink annoyances to deal with. In project pages that are particularly laden with JavaScript, I take the time to write links with the accompanying switch mechanism off in order to leave turbolinks on globally.

Turbolinks can feel pesky. The exercise of forcing myself on them required of me that I learn their behavior a bit better, exactly what I wanted. I found how in the Chrome browser the behavior is most present. When writing for Wordpress, I like to use Chrome for surfing its administrator management screens. I watch upload progress in the status bar. I like FireFox for testing the front end and drilling into computed code with its terrific inspector. I like Safari for its default on the Mac operating system, another example of my forced learning behavior. I can manage system and site notifications. I occasionally use Opera purely for its distinction.

People tend not to notice things as readily as when they have contrasts to compare, or when a familiar process breaks down and a page refresh is required. When this occurs at a seemingly odd times, it could really be a result of practically anything. It is one of the tell-tale signs of turbolink behavior in Chrome that I notice when working on a Rails 4+ project. This occurs for me not only in Rails projects, now I have noticed the same behavior in the administrator screens of Wordpress. I am all for making static page components stick and only changing those bits that require alteration. I especially notice when I think it is broken turbos.
