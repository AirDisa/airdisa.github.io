---
layout:    post
title:     Using Jekyll Exclude
excerpt:   When you do not want to be powered by Jekyll.
date:      2014-04-01 21:14:36
published: true
category:  jekyll
tags:      jekyll
---

This file will be excluded from processing by Jekyll. Since this is a markdown file, I presume other file types also can be excluded which would otherwise be processed by Jekyll, including by way of example at divshot, the JSON format. Notice the exclude method in _config.yml points to the _posts folder, presumably other folders and perhaps file types located in root or wherever. I wonder how this all will work out. Only experimenting will tell. I will leave this file as in the original, so that I can detect where it might get triggered and by what process if these things ever appear.

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Disa')
#=> prints 'Hi, Disa' to STDOUT.
{% endhighlight %}

[jekyll]: http://jekyllrb.com
