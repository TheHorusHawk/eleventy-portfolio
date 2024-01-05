---
title: "New project: Legal Register"
description: "Description of new Django project, a legal register"
date: 2024-01-05
tags:
  - Django
  - Virtual Environments
  - Postgresql
  - bash_aliases

---
I have just started a new web application, a Legal Register. It's a way for organisations to know what laws and regulations they have to comply to. 

I started by creating a virtual environment, and immediately ran into trouble. I wanted to use the most recent version of django (because why not) and it required I download a more recent version of python. So far, so good.

Except, though I created the virtual environment via the newest python version (3.12), inside it, when I ran `python --version`, I always got my distribution's basic python3 version, version 3.8. What gives? I tried using virtualenvwrapper, virtualenv and venv. Always the same problem. Googling it gave no answer, it seems like I was the only person in the world having that issue. Well, that's not good! If stackoverflow can't help, what can?

And then I checked my `.bashrc` file. And, yeah... So, embarassingly, a younger, less experienced me - one who hadn't heard of virtual environments - had grown tired of writing python3 everytime he needed to run something in python from the terminal (stuff like `python3 manage.py runserver`, and other basic django commands) and decided to add this line `alias python='/usr/bin/python3'` to his `.bashrc` file. 

So, regardless of what the python version in the environment was, either globally, or in the virtual environment, I had taught that, if I write `python` I mean `/usr/bin/python3`. And that was python 3.8.

So, is that fun, enlightening or just plain foolish? For me, it's learning, and frustratingly long as it has been to develop the most basic of setups (it took me an afternoon just to get a basic user/authentication thing going), I deepened my knowledge of the tools I was using, and gained the confidence to persevere in the face of a seemingly intractable problem right at the outset of a new project.

Since I'm hoping to scale this project up later, I decided to use a postgres database rather than the django default, SQLite. So I did a tutorial and set up django to work with the database. That was pretty easy (Django is officially supported to work with postgres) but it still involved me writing a few lines of SQL code, which felt pretty cool, somehow. And it works. So that's one more thing I know how to do. Ish. Until it crashes. But, if/when it does, I'll keep at it, deepen my knowledge and figure it out in the end.

Oh, and I have succesfully configured a login, logout and signup for my application. All in all, a good day.
