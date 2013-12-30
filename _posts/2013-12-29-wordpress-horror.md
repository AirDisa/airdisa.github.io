---
layout:    post
title:     Wordpress Horrors
excerpt:   What is meant by Wordpress horrors?
date:      2013-12-29 15:32:30
published: true
category:  wordpress
tags:      wordpress
---

As mentioned before, you are bound to run into Wordpress during your life as a developer. If you are lucky, you get to avoid Wordpress horror, or you become so familiar with Wordpress that they no longer bother you. There is little room for life in between. I think I was comfortable knowing little about Wordpress while I was perfectly able to live life without it altogether. Those days were numbered and I have had to begin life on the opposite side of the spectrum.

Here are some nits that I will complain about Wordpress. Unless I install it on my machine, finding a good work flow is extremely time-consuming if you are doing anything more complicated than using the built-in code editor. There are fields where edits can contain bits like PHP to plug in to the core, or where you can add whatever the container will allow by way of code you can use to accomplish something. I got away with this work flow for years without running Wordpress locally.

Whenever I code a theme or plugin and Wordpress is not installed, I quickly pay a time toll tax. That is, editing code using built-in fields only take you so far. Full-blown theme or plugin design is best done with a running copy of Wordpress. I really dislike this, it makes me irritable. I reserve my machine for other projects including running my business. I might install Wordpress in a gated cloud somewhere, if work warrants it. The point is I do not *want* to install that nasty thing anywhere.

{% highlight php %}
<?php the_content( $more_link_text, $stripteaser ); ?>
{% endhighlight %}

[Wordpress documentation][codex] says this has to be run in [The Loop][the_loop]. Seriously? This is where a picture materializes for me that Wordpress is a maze of loops, includes and conduits for the blog, its themes and plugins with daft PHP methods names like the content and stripteaser params which must be used in a loop where you expect post excerpts because everything is disoriented context-oriented striptease catcalls in the loop. Memorize it but it sure is nice to be blissfully unaware.

That is only where decision horror begins. Loops and includes from a maze of directories separated between core code, theme code and plugin code quickly overwhelms any better sense of organization. There is always rationale (excuses!) behind the myriad hooks. Jekyll is a simple thing of beauty compared. Rogue galleries of criminally-coded plugins and themes giddy people innocently install too easily, a galaxy of veritable malware. Find hidden base64 encoded links to casinos!

Exercising caution is fine, except it steals your time, the life-force. It takes time to memorize the mazes to know your way around Wordpress. Once you become known for Wordpress, forever will it dominate your destiny. Watch out if you do not want to be known for handling it well unless you are prepared to take the work. There is plenty to do too, plenty of horrors, nightmares for the unsuspecting. Wordpress horrors is why there is tons of Wordpress work. That is what is meant by my headline.

[codex]: http://codex.wordpress.org/the_content
[the_loop]: http://codex.wordpress.org/The_Loop
