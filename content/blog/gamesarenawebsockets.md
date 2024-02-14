---
title: "Games Arena: Web Sockets"
description: "Update on my games arena project"
date: 2024-02-14
tags:
  - Django
  - Web Sockets
  - Django-channel
  - ASGI
  - Redis

---
Hey,

Quick update on my Games Arena project, a server that allows people to play games (When I say "games", I mean Tic Tac Toe). I was struggling to implement a feature where the board updates when the oponent's made a move.

After reading on some quick fixes, I decided to dive right in and do it well, though it was a lot more trouble than having, say, JavaScript ping the server from time to time to check if there's updates.

I implemented it via web sockets. To do that I got Django-channels, and used it to implement a simple page reload when there was an update (the code already takes care of everything else.)

I didn't know anything about web sockets before this. So I did a tutorial on building a chat server. Then, I pasted and modified some code to do what I wanted it to do (I didn't want it to be a chat server, just to update the page).

I'm very happy that it's working. But it's also made me think about what it means to understand something more generally.

Though I read the tutorial text carefully, I really cannot claim in any way to understand the underlying code. I have successfully manipulated it to do what I wanted it to do, so there's enough understanding for that, but it's not even good code at this point, and it's inefficient (I couldn't quite remove the need for the underlying code to send a dummy message in order to activate the reload, for instance). I will seek to clean it up in the future, but it's still the work of someone who's more knowledgeable than me (the one who wrote the tutorial), really.

That's what got me thinking, I use a really high level framework, Django, anyway, that abstracts away most of the complications of the web. That I'm able to kind of manipulate that doesn't make me someone who understands the web either. It feels like it's whoever programmed Django that understands the web. Or is it the people who programmed the underlying structures on which Django runs?

We can go all the way down. The joke is if someone claims to know how to build something with computers, throw some sand at him and tell him to go make a computer first.

I suppose it's just the way of engineering, the whole standing on the shoulders of giants thing, building on what the community of programmers has built, and on their understanding, that makes the whole enterprise (programming) possible. But, while it makes me wonder about its resilience, its capacity to withstand shock, etc., I'm mostly concerned about myself (surprise!), of what it means to require a vast human and industrial base for me to do the simplest things, if it wouldn't be better to get to know something very deeply, and what it means to know things deeply, really, when we are all kept afloat on massive amounts of knowledge that have been passed on to us? Not only in computing but in basic necessities to support life. For instance, sure, we know how to buy food, but who knows how to grow it anymore? What about our houses? We may know how to install some things, but who knows how to build anything? I'm sure the knowledge is out there, it just made me thing how deeply I depend on vast amounts of people I have never seen.

Musings aside, it was quite fun. Whenever I'm faced with something new, I go through stages of "Don't want to learn" through persevering into excitement at the thing I did being functional. It's always a great feeling when that happens, especially as you get to say "I told you so" to the part of yourself that thought it was impossible!

And that's it. Happy valentine's day!