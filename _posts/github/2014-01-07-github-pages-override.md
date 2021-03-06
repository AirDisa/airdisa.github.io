---
layout:    post
title:     GitHub Pages Override
excerpt:   Latent Semantic Indexing gotcha
date:      2014-01-07 06:01:28
published: true
category:  github
tags:      github
---

Taking advantage of the speed with which one can get up and running on Jekyll with GitHub Pages left me open to forgetfulness about what they override. Part of this was intentional, since the fun was really wrapped up in learning Jekyll quick and running it. I poured a goodly amount of time into hammering the little nits I thought were getting in the way of getting LSI to publish related\_posts to GitHub Pages using the Jekyll plugin. I had seen warnings about their use of --safe on build, with conflicting advice elsewhere that you can still run plugins and publish the output as long as you run the build first, of course with --safe and LSI set false.

<blockquote class="twitter-tweet" lang="en"><p>Running ~$ jekyll serve with LSI set true in _config.yml populates related posts accordingly. GitHub Pages --safe flag ignores LSI. Aw well.</p>&mdash; Disa Johnson (@AirDisa) <a href="https://twitter.com/AirDisa/statuses/419608370455117824">January 4, 2014</a></blockquote>

More precisely, documentation on [configuring Jekyll][config-jekyll] state these overrides:

{% highlight yaml %}
safe: true
lsi: false
pygments: true
source: your top-level directory
{% endhighlight %}

It makes sense for security reasons to run Jekyll build in safe mode. It also makes sense to override the top-level directory option so your site works. It makes sense to disable LSI and pygments for their processing hardship. In the case of LSI, there are Linux package dependencies too. I read through these warnings quickly around Christmas time, when Jekyll was like a present under the repo tree. I was having so much fun that I wrongly presumed I could run build with LSI locally, then git push. Not so. I neglected to see in my head they would still build and overwrite. Once that became clear, I came across this [Rakefile][rakefile] workaround:

{% highlight ruby %}
require 'fileutils'

    task :publish do
      FileUtils.rm_rf('/tmp/airdisa-index')
      ENV['GIT_INDEX_FILE'] = '/tmp/airdisa-index'
      sh "jekyll build generated"
      sh "cd generated && GIT_DIR=../.git git add ."
      tsha = `git write-tree`.chomp
      csha = `echo 'updated' | git commit-tree #{tsha}`.chomp
      sh "git update-ref refs/heads/master #{csha}"
      FileUtils.rm_rf("generated")
      sh "git push -f origin master"
    end
{% endhighlight %}

This looks like some serpentine fun! I edited to add a build directive and removed the --lsi flag, since I presume having LSI set true in \_config.yml should naturally work. I have not yet tried this. I marvel at the possibilities of which this is one. The idea centers around a forced push with an alternate index and branch with a local LSI build to a generated folder. It also meddles with git shas Pages will point to the unparented branch. I am wary and weighing this against that it might not work, or some time in future it fails to. A policy change down the line and content might not make the trip at Pages. It looks fun to explore before Octopress 3.0 though:

<blockquote class="twitter-tweet" lang="en"><p><a href="https://twitter.com/anandrajaram">@anandrajaram</a> It’s under active development, but the current release is about to be replaced. Use Jekyll, and check us out again at 3.0.</p>&mdash; Octopress (@octopress) <a href="https://twitter.com/octopress/statuses/416396115861585920">December 27, 2013</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

[rakefile]: http://www.trottercashion.com/2011/04/11/use-git-plumbing-for-more-awesome-github-pages.html
[config-jekyll]: https://help.github.com/articles/using-jekyll-with-pages#configuring-jekyll
