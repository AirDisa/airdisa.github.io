---
layout:    post
title:     Wordpress Horrors
excerpt:   What is meant by Wordpress horrors?
date:      2013-12-29 15:32:30
published: true
category:  wordpress
tags:      wordpress
---

As mentioned before, you are bound to run into Wordpress during your life as a developer. If you are lucky, you get to avoid Wordpress horror, or you become so familiar with it that it no longer haunts you. I find little room for life in between, myself. I think I was comfortable knowing nothing about Wordpress. Those days were numbered. I have had to begin thinking on the opposite side of the spectrum.

Here are some nits that I will complain about. Finding a good work flow can be extremely time-consuming if you are doing anything more complicated than what an be done with the built-in code editor. Even so, the editor only offers clumsy going. When I code a new theme or plugin and Wordpress is not installed locally, I quickly pay a time toll tax.

I try to reserve my machine for running my business. It makes me irritable to run anything that is not related to that essential set of tasks. A development machine can live too close to the edge, where project problems might interfere with day-to-day operations. When work warrants it, then I need to install something. The point is I do not *want* to install anything.

{% highlight php %}
<?php the_content( $more_link_text, $stripteaser ); ?>
{% endhighlight %}

[Wordpress documentation][codex] says the content method has to run in [The Loop][the_loop]. This is where Wordpress mazes and loops materialize. PHP methods named the content, params named stripteaser running in The Loop, you can only use this stuff where you expect post excerpts because as global sounding as the content is, it is purely a red light district striptease just for those contents in the loop.

Memorize this maze if you must, but it sure is nice to be blissfully unaware of such horror. Any sense of organization can get overwhelmed by the madness of it. There is rationale (excuses!) behind everything but Jekyll is a simple thing of beauty compared. Let us not forget the rogue gallery of criminally-coded themes and plugins. Instant base64 encoded links to casinos!

[codex]: http://codex.wordpress.org/the_content
[the_loop]: http://codex.wordpress.org/The_Loop
