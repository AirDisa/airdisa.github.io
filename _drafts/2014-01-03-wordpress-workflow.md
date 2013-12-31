---
layout:    post
title:     Wordpress Themes
excerpt:   Writing Wordpress themes (to get the feel for madness).
date:      2014-01-03 08:24:48
published: false
category:  wordpress
tags:      wordpress
---

Unfinished.

Details about how to go about working writing a Wordpress theme the way I do has not been properly explained. Now that I am in the mood, I will share those details which I hope people starting out will appreciate someday. My first recommendation is to get familiar with command line coding, the sooner you do, the better you will be faster. It can be a steep learning curve that is well worth it once you find the slope begins to work in your favor instead of working against you. Even while I worked in Windows for decades, I left it behind solely for Linux.

If you are struggling with wanting to know more and put off that I no longer use Windows in my worflow, take heart knowing you can always Telnet or Putty into a Linux machine for rent at less than a dollar a day, one that is in the cloud ready to serve code over the Web. Learning that may actually convince you to switch but it is entirely up to you if and when you decide to do so, if you should decide to do so. There is nothing like the freedom to know that you have options. Windows is perfectly suitable and required at some companies, so knowing it is important too.

There are developer opinions, charged up opnions, about which text editor is best. I like the idea of a text editor that increases my capability on the command line, and therefore I choose Vim. Many prefer Emacs or a commercial product like Sublime. Whatever you choose for an editor, I recommend Vim or Emacs since these are going to reinforce your learning command line utilities on Linux. I say Linux but really any Unix-based operating system would probably do regarding my workflow. I am running Ubuntu, a Linux distro at Linode in the cloud from a Mac or iPad at home.

In the case of Linux my sessions always start with a Bash shell. To launch on the Mac I use cmd-space for Spotlight and type the letters iterm until the program is found and hit enter to start it. Once there, I will launch ssh (secure shell) to the IP at Linode which after user pass credentials will launch me into bash on the Linux machine in the cloud. The nice thing here is the consistency of Bash. It will be the same in the cloud as it is at home on my Mac. If you are on Windows, you will need to switch gears depending what you are doing.

Once in the cloud, after having set up my machine as root and configuring myself as a normal user, I boot in to the normal user from them onward. I can install packages with sudo, which is short for: super user do. That way I can install and configure GitHub so I have version control. From then onward, everything I do is fairly normal for managing packages, writing code and publishing to the Web. If all this seems way too complicated and scary, just remember no one is hurt by you firing up your own instance and experimenting. The world will keep spinning.

[linode]: http://linode.com
