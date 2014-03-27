---
layout:    post
title:     Meteor Shower
excerpt:   The Meteor framework based on Node is pure JavaScript
date:      2014-03-22 21:56:53
published: true
category:  meteor
tags:      meteor
---

I first came across Meteor last fall, and the video got to me pretty good. Although I had a job to do through Christmas, I meant to get to checking out Meteor after the Holiday in the first part of 2014. Here we are. Now that I have had a look, I really like what I found and look forward to the framework getting to version 1.0. I know that it is backed by some VC capital (roughly $17m I think, by Marc Andressen) so it has some resources behind it and is not therefore a garage project.

The thing that I think is great is that Meteor is reactive, meaning that changes are pushed up the wire (fibers) to the browser so the user experience is super fast, with little to no network latency. This is accomplished with a trick. Changes on screen can take place even before the change is accepted by a database, and stick only if the change is ultimately accepted, which normally it would be - so why not make this a seamless experience for the user? Great idea.

What is really nice is that most frameworks utilize a mix of languages to accomplish the whole that is modern MVC app architecture. With Meteor on Node it is pure JavaScript, from the Node back end server-side code, to the front end code and the data store is Mongo all through JavaScript JSON API. There is a template engine which comes with Meteor, handlebars, so you get the capability of variable-driven dynamic front end code too. Handlebars is easy to use, which is good, since I had not used it before.
