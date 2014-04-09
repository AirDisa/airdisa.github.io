---
layout:    post
title:     Heartbleed OpenSSL Bug
excerpt:   A zero-day vuln revealed after nearly two years.
date:      2014-04-09 12:12:20
published: true
category:  security
tags:      security
---

Oh boy. This is a big bug that affects websites that use OpenSSL which is pretty much everyone doing authentication. Big sites like Twitter and Google are patched up and no longer vulnerable. It was Google researchers who uncovered it. There is little question that industrious hackers have been using it to compromise systems, or at least there is no question we all must assume so. The Microsoft camp finally have a flaw that points away from their architecture.

Glee for them. What is happening?

A flaw in the OpenSSL heartbeat handshake, a &quot;hello are you there, service?&quot; exchange, allows the attacker to prompt for up to 64k in the clear. The data will come from active system memory, where one of the most important secrets are kept. The attacker is not limited to the mumber of times they can prompt, collecting samples of info until they have the certificate key itself so they can crack everything encrypted using that key. They can retrieve passwords along the way too.

OpenSSL is so widely used that the half-joking suggestion to users is to stay off the Internet. For once, this is actually pretty advisable - at least avoid doing any banking while the criminals do their best to exploit as much as they can to compromise systems before the script stops working. After a time, it will be very important to change your passwords ([you do have different passwords for every service, right?][passwords]), but you should only do this after the website has changed certificates.

All this will be so complicated for the average Jane on the Web. It is definitely interesting to watch. One thing that is pretty easy to assume is that governments have probably known about this for a time, and probably used it to crack open some boxes. Times are definitely tough in the world of cryptography, since hashing algorithms have backdoors, secure certificates get spoofed and now this makes it so easy that you would think there is no security, which is what we have known for some time.

[passwords]: http://airdisa.github.io/security/2014/01/09/secure-passwords.html
