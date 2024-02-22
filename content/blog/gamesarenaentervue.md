---
title: "Games Arena: Enter Vue"
description: "Django web application, second week update."
date: 2023-10-05
tags:
  - Django
  - Web Application
  - Python
---
So, this week, I finished implementing the feature of setting a player as online and not online via middleware and caching. They way it's implemented, there's a list of all the player who are online - defined as having interacted with the application in the last 5 minutes - on the cache at all times, which is updated by the middleware.

The function that renders the template then works out who isn't online and feeds both lists to the template. The webpage then shows two lists, one with the players who are online and another with the players who are offline. Sweet!

Time for some frontend. I now need to implement a way for players to interact with other players and challenge them to games. I wanted to use Vue.js, a library, rather than vanilla Javascript, which I have no experience with. So, I've been reading documentation and doing tutorials.

As for what's next, I have to implement the interactions. I'll start by implementing a button next to the name of a player with something like "Challenge to game". I'm not 100% sure I'll be using Vue, but, if I do, I'll have to configure the application to use it.

I'll let you know all about it on my next update!
