---
layout:    post
title:     Jekyll Folders and Google Indexing
excerpt:   The best time to lay the architecture foundation is early.
date:      2014-04-05 09:46:20
published: true
category:  jekyll
tags:      jekyll
---

I moved posts because they were getting too numerous. Leftover anxiety about Google Indexing from my career in search was amazingly holding me back. As a flat file site I am keen to watch its indexing. As an experimental platform (Jekyll versus other experiments I have conducted with the likes of Perl etc.), I wanted to watch how things go and figure things out like redirecting. All this was silliness. As a flat file system, indexing is going to be perfect suited to Google and all else. As a new platform though, I learned a couple things I can articulate here that may be of interest.

My concern began early when I first began trying out Jekyll last Christmas (2013). I learned fast and cannot dedicate too much time to learning since I have plenty of commercial work to do, and none of it is with Jekyll - yet! Posts would quickly become too numerous for the _posts folder to manage very easily, navigated in Vim by way of using the forward or backward search patterns to find a specific file just inconvenient for any editor to have what can amount to dozens, then potentially hundreds of files occupying a single folder. Presumably, I could file them all away in folders. Naturally done, and can redirect.

There is the issue that I do not want to use my own host provider in this case or it would be simple enough. The trouble thinking this through really comes about using GitHub as a host provider, which is very germane to my experiment. I want to be able to have knowledge of a system that is ultimately free from all fees, something where a clever person with only access to a local machine and the Web can do some fairly neat things with little else and no commercial host mickey mouse malware inserts. At least GitHub can be counted on as a host provider and the user really only need to learn the fairly simple Jekyll publishing platform.

I looked into all these things only to eventually discover how simple it really is. Apparently, the folders in the _posts directory are not processed by the Jekyll engine at build time, which means the directory structure and pathname is entirely left to YAML and Jekyll. I had spun my wheels on redirecting, since .htaccess is impossible at GitHub in this case, and everything in _posts is processed which meant that trying to include a refresh file at the original location ends up in pagination - all manner of horror like that! I went ahead and wrote a flat html file in the root directory and passed variables to a meta refresh template.

All this for nought. It turns out that - I strangely remember noticing this earlier, just forgot - that you can organize your files any way you like. The Jekyll engine will only process files with YAML markdown and Jekyll ruby methods in them regardless of how you organize everything before the processor. One clue I had which I failed to see was the generated site had the folder names as defined in the YAML when the markdown remained in the _posts directory. Silly me, I should have noticed this and been clued in. I may be pretty good when I am wide awake. It is in the off times that I am not working I get to hack Jekyll with half my brain.

Now that I have figured all this stuff out, I went ahead and tried a few things. Correct me if I am wrong and you know better but I was able to accomplish excludes by way of the exclude statement in the _config YAML file, as well as notice that files and folders named with exclude which appear in the _posts directory also do not get processed by the Jekyll build engine. It seems to be fairly straight forward and I think that is enough to go by. It provides several methods to exclude stuff and I left a few files in place which use these schemes except the file named exclude opting to demonstrate the exclude statement in _config in lieu of that.
