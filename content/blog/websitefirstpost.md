---
title: "Website: New project using Pelican"

description: First update on new project, creating a website using Pelican 
date: 2023-09-01
tags:
  - Static website
  - Pelican
---

I'm making a static website in which to keep the creative parts of my internet presence organised.

I'm using Pelican, a Python static website generator, and Markdown for the pages. Pelican is very easy to use. Having written websites in clunkier ways (my previous website, which dates from the early 2000s, was written entirely on raw HTML) I found it a breeze to create the content, layout and articles. 

Documentation is short and very well written, with about everything you might need from a website like this. It lends itself to being configured to automate lots of things (such as the article type, category, date of publication and modification) as well as automatically reacting to a new file and, making the output HTML and serving it. So, after just a few tweaks, you're just writing really simple markdown files and saving them. This is a way of working I appreciate, but I'm also reassured I can change the fields being written automatically by manually including them, which I have been making use of to create an archive of past projects based on when I first released them, rather than the date of creation of the article.

This week, I've initialized my project, configured it to do what I need it to do, been trying out different themes and different functionalities. I like the way there's a base configuration that gets changed based on a smaller, easily readable file (at least so far, as I haven't changed that many parameters) which sets out what you need for testing and that there's a further file with config for when you actually go ahead and publish it. So far, it reads well and works well. Haven't brought it live yet, though, as I want to flesh out the content a little better before I do that, so I'll put a note here detailing how that went

I've also been using virtualenv to create a virtual environment where I have installed pelican and markdown. This is something I plan to do going forward on other projects, as it is a much neater way to ensure you have what you need for a particular usecase without messing with other projects. I will be using that on the web app I'm developing as well, especially as I'll be working with a database (Redis) which I haven't used before, and I want to make sure I don't break things in the base configuration.

That's all for now!
