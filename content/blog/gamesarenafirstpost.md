---
title: "Games Arena: New project first week update"
description: "Django web application, project name 'Games Arena', week one update."
date: 2023-09-21
tags:
  - Django
  - Web Application
---

I'm starting a new project in Django, which is to be the final project of my Web Development with Python and Javascript course. Unlike other projects of that course, this one I will be doing from scratch, with no seed code. 

This first week, I have initialized the django project and created a screen to choose your nickname. Once you do, or if you already have logged in before, it will take you to the Games Arena proper, where you'll be able to see who else is online so you can choose people to play a game. All this is done via sessions.

At the moment, being online is implemented only as a button which allows players to make themselves available for a game, but I'm looking to implement a way for the server to tell who is and isn't online automatically. I'm looking to do this via Redis. More news on that, or on my failure to do so, on my next update, I hope.
