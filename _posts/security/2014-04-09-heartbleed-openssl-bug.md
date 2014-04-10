---
layout:    post
title:     Heartbleed OpenSSL Bug
excerpt:   A zero-day vuln revealed after nearly two years.
date:      2014-04-09 12:12:20
published: true
category:  security
tags:      security
---

The OpenSSL HeartBleed security flaw is a big developer bug that affects the ubiquitous TLS (transport layer for securely encrypted data exchange) used by websites, pretty much all of them doing anything like authentication which is anything like logging in. Sites like Twitter and Google are patched up and no longer vulnerable. It was Google researchers who uncovered the flaw in the first place. There is little question that hackers have can use it to compromise systems and we must assume they have done so.

Microsoft finally have a flaw that points away from their architecture. Glee for them. What is happening? A flaw in the OpenSSL heartbeat handshake protocol, a &quot;hello are you there, service?&quot; small exchange that is meant to verify (or keep warm) connections allows an attacker to prompt for up to 64k in the clear by spoofing its own size. In response, the hearbeat transmits back what is meant to be the original message stored in memory up to 64k. The black hat trick here is to spoof the hearbeat request size.

When an attacker spoofs the size of its message to 64k (when in actuality it can be 1k) when the heartbeat samples its memory of the original message it includes extra data from memory, which includes all the sesnsitive stuff since it is the proptocol that governs security. Worse still, the attacker can generate as many spoofed requests as they like and leave behind no meaningful trace of activity. It is a free for all fall down lapse of security when the attacker gains the prized target of the system encryption key.

Once a system gives up its certificate key, the attacker can then crack anything encrypted on that system. They can retrieve passwords along the way too, since the encryption key may not be the first thing they come across. Again, there is no limit to the volume of requests an attacker can make, and therefore it is only a matter of time until that windfall key comes into their possession. That is what makes this security flaw so endlessly perilous until patched up. Criminals are likely using the flaw now for last attempts to steal.

It is very important that users change passwords ([you do have different passwords for every service, right?][passwords]) but only do so after websites have newecure certificates for encryption. Assume all your old passwords will be part of tables used in brute force attacks and rainbow seeds for algorithms that crack stolen hashes which remain encrypted afterwards. That means that the problem is not over once websites have patched OpenSSL and refreshed their certificate keys.

<blockquote class="twitter-tweet" lang="en"><p><a href="https://twitter.com/janl">@janl</a> <a href="https://twitter.com/marihuertas">@marihuertas</a> Three ordered things needed: 1) Patch OpenSSL 2) New cert to generate new server-side keys then 3) user changes password.</p>&mdash; Disa Johnson (@AirDisa) <a href="https://twitter.com/AirDisa/statuses/453878257784340480">April 9, 2014</a></blockquote>
<blockquote class="twitter-tweet" lang="en"><p>ICE: Software developers can recompile OpenSSL with the handshake removed from the code by compile time option -DOPENSSL_NO_HEARTBEATS.</p>&mdash; Disa Johnson (@AirDisa) <a href="https://twitter.com/AirDisa/statuses/453883430116528128">April 9, 2014</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

[passwords]: http://airdisa.github.io/security/2014/01/09/secure-passwords.html
