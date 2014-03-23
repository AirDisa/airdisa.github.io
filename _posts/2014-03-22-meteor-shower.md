---
layout:    post
title:     Meteor Shower
excerpt:   The Meteor framework based on Node is pure Javascript
date:      2014-03-22 21:56:53
published: true
category:  meteor
tags:      meteor
---

I first came across Meteor last fall, and the video got to me pretty good. Although I had a job to do through Chirstmas, I meant to get to checking out Meteor through the whole Holiday and into the first part of 2014. Now that I have had a look, I really like what I found and look forward to the framework getting to version 1.0. I know that it is backed by some VC captial (roughly $17m I think, by Marc Andressen) so it has some resources behind it and is not therefore a garage project.

The think that is great is that is reactive, meaning that when changes are pushed up the wire, or fibers, to the browser so the user experience is super fast with little to no network latency. This is accomplished with a trick, that changes on screen can take place even before the change is accepted by the database and will stick only if the change is accepted, which normally it would be - so why not make this experience as seamless for the user as possible? Great idea.

What is really nice is that most frameworks utilize a mix of languages to accomplish the whole that is modern MVC app architecure. With Meteor on Node it is pure Javascript, from the Node backend server-side code, to the frontend code and the data store is Mongo all through Javascript JSON API. There is a templating engine which comes with Meteor, handlbars, so you get the capability of variable-driven dynamic frontend code too. Handlebars is easy to use, which is good, since I had not used it before.
