---
layout:    post
title:     Wordpress Horrors
excerpt:   What are my Wordpress horrors?
date:      2013-12-29 15:32:30
published: true
category:  wordpress
tags:      wordpress
---

As mentioned before, you are bound to run into Wordpress during your life as a developer. If you are lucky, you get to avoid Wordpress. You can always learn it and become familiar enough with the horror that it no longer frightens you. I found little room for life in between once the madness started. I think I was comfortable knowing nothing about Wordpress. Those days were numbered. I had to begin thinking on the opposite side of the spectrum. Here are some nits that I will complain about. Finding a good work flow can be extremely time-consuming when I plan on doing anything more complicated than what can be done with the built-in editor.

The editor is clumsy going. When I code a theme or plugin and Wordpress is not installed, I pay a time toll tax. I successfully avoided installing it as yet and the more I get related work, the more I can no longer avoid installing and running it on a machine. You still need to browse Wordpress. The efficiency you buy by having it installed is that you no longer need to wait for processing uploads of the zip archive it wants for themes and plugins. I like hot fixing code, so this suits my workflow fine. I do not enjoy the hassle of setting up Wordpress or anything I am not personally committed to using, except clients demand it.

{% highlight php %}
<?php the_content( $more_link_text, $stripteaser ); ?>
{% endhighlight %}

[Wordpress documentation][codex] says the\_content method has to run in [the\_loop][loop]. This is where for me Wordpress turns into a carnival, complete with laughing clowns. There is nothing scarier than evil clowns. I often run away leaving my frenzied code behind to return later. As global sounding as the\_content is, it is confined in scope. Params could be better named than stripteaser. There is rationale (excuses) behind everything Wordpress does but Jekyll is a such a thing of beauty compared. Learn Wordpress if you need in order to work it. It sure is nice to be blissfully unaware. Let us not forget free plugins you can install. Instant base64 encoded links to casinos!

[codex]: http://codex.wordpress.org/the_content
[loop]: http://codex.wordpress.org/The_Loop
