---
title: "Games Arena: Update"
description: "Django web application, project name 'Games Arena', week one update."
date: 2023-09-28
tags:
  - Django
  - Web Application
---
You know when you're going through something, and you realize you have to do something else before you do that, and you do that hoping it's not going to take long, and while you're doind that something else you bump into something else that you also have to investigate? If you've ever read David Foster Wallace and got sucked into a footnote midsentence and realised that footnote is a massive text with its own footnotes, you know the feeling I'm describing.

That's how it's been going for me. This past week I have decided to implement a "is online" feature to check which of my players is online. So I decided to do it via cache, and that has led me to do a tutorial on caching with Redis, which is a cached database, and of course this tutorial was broken in newer versions of Python/Django, so I've decided to use a virtual environment just to do the tutorial, so that's got me to research into how virtual environments work and once I've got it to work (via a different workaround, as it turned out), I learned a cool node tool called loadtest, then  I realised I had to implement it as middleware, so I've been seeing how to do that. In the process I also learned a bit about the intricacies of how to implement many-to-many relationships in django.

So, all-in-all, maybe three lines of code written per hour spent reading documentation. But that is not to say it's been a bad week, just one in which I got to go deeper and learn really important foundational elements for the work ahead, and future workings with the tools. It's been a great week, actually, and it's felt like I keep overcoming obstacles and getting more knowledge as a result. Hazzaa! It's weeks in which it seems I can't make headway, and I'm not learning anything, which I dread.

So, I've got a really nice and functional middleware. It doesn't do much, yet, that's for later, but I hope I'll be able to park this one item soon. I'm still on a single item on a spec: implement "is online". I will be phewing hard once that is done.
