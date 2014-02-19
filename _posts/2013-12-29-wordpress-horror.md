---
layout:    post
title:     Wordpress Horror
excerpt:   My Wordpress horror?
date:      2013-12-29 15:32:30
published: true
category:  wordpress
tags:      wordpress
---

You are bound to run into Wordpress as a developer. I was too comfortable knowing nothing about Wordpress, thinking of it as a glorified guest book. I successfully avoided lost time in the madness of its admin screens. Those days were numbered. I had to use Wordpress for client work. Aw well. The editor is clumsy. The workflow is a terrible wait for zip archive uploads of awful themes and plugins.

{% highlight php %}
<?php the_content( $more_link_text, $stripteaser ); ?>
{% endhighlight %}

[Wordpress documentation][codex] says the\_content method has to run in [the\_loop][loop]. This is where Wordpress for me turns into a carnival. After I fight my way through a file permissions nightmare to hack files directly, core code contains juvenile jokes like laughing clowns. Params named stripteaser? There is nothing more frightening than laughing clowns. As global sounding as the\_content is, it is small in scope.

Jekyll is a such a thing of beauty compared.

[codex]: http://codex.wordpress.org/the_content
[loop]: http://codex.wordpress.org/The_Loop
