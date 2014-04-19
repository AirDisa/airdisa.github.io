---
layout:    post
title:     Heartbleed OpenSSL Bug
excerpt:   A zero-day vuln revealed after nearly two years in the wild.
date:      2014-04-09 12:12:20
published: true
category:  security
tags:      security
updated:   2014-04-19 12:10:00
---

The OpenSSL Heartbleed business is a security flaw so major, that it affects pretty much all websites doing membership authentication and e-commerce. Google researchers uncovered it recently, but the there is little doubt that hackers have been using it to compromise systems since last November. We must assume they have done so with our own websites and get the fix in. The flaw is the OpenSSL Heartbleed handshake, a &quot;hello are you there, service?&quot; exchange meant to verify (or keep warm) connections was subject to spoofing.

The flaw allows an attacker to retrieve up to 64k in the clear by spoofing its own request size, the Heartbleed transmits back what is meant to be the original message stored in its own memory, up to 64k. The black hat trick here is to spoof the size with a script as little as 1k and get back 64k. The message includes all the sensitive data you would expect to be encrypted. An attacker can generate as many spoofed requests as they like, enough to trick the system into giving up its actual security certificate key and leave behind no trace.

Once a system gives up its certificate key, the attacker can then crack anything encrypted on that system. It is very important users change passwords ([you do have different passwords for every service, right?][passwords]) but only do so after websites have gotten new secure certificates. Assume all your old passwords will be part of tables used in brute force attacks and rainbow seeds for algorithms that crack stolen hashes. That means Heartbleed will still be a problem even after websites have patched OpenSSL and gotten new certificate keys.

<blockquote class="twitter-tweet" lang="en"><p><a href="https://twitter.com/janl">@janl</a> <a href="https://twitter.com/marihuertas">@marihuertas</a> Three ordered things needed: 1) Patch OpenSSL 2) New cert to generate new server-side keys then 3) user changes password.</p>&mdash; Disa Johnson (@AirDisa) <a href="https://twitter.com/AirDisa/statuses/453878257784340480">April 9, 2014</a></blockquote>
<blockquote class="twitter-tweet" lang="en"><p>ICE: Software developers can recompile OpenSSL with the handshake removed from the code by compile time option -DOPENSSL_NO_HEARTBEATS.</p>&mdash; Disa Johnson (@AirDisa) <a href="https://twitter.com/AirDisa/statuses/453883430116528128">April 9, 2014</a></blockquote>

<blockquote class="twitter-tweet" lang="en"><p>Tor begins blacklisting exit nodes vulnerable to <a href="https://twitter.com/search?q=%23Heartbleed&amp;src=hash">#Heartbleed</a> <a href="http://t.co/xosji55rd2">http://t.co/xosji55rd2</a></p>&mdash; Eugene Kaspersky (@e_kaspersky) <a href="https://twitter.com/e_kaspersky/statuses/457170509105332224">April 18, 2014</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

[passwords]: http://airdisa.github.io/security/2014/01/09/secure-passwords.html
