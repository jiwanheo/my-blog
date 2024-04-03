---
title: 'Fullstack app [Part 1]: React frontend'
author: Jiwan Heo
date: '2024-04-02'
DisableComments: no
---

In this post, we'll make a simple bookmark app. Users will be able to save a URL
of a webpage they like, and view it later through this app!

Users will see 3 things in this app

- A form to enter and save URL
- A front page UI for seeing the most recent bookmark
- A table UI for seeing all the bookmarks

So this is 1 POST request, and 2 GET requests - one for seeing the latest 
bookmark, and another to query n number of bookmarks (maybe this can be one, 
with parameter).

## Set up

Let's use vite as our build tool, and start a project called "bookmark-app". Run

`npm create vite@latest bookmark-app`. 

It's going to ask to install package and select
a few options. I'm not going to do anything fancy and go react/javascript.

![](vite-setup.png)

I'll run the code suggested in the terminal. If you see this screen, you did it 
correctly!

![](vite-setup-done.png)

## Dev

Let's open this directory in vscode and do some dev'ing. Run `code .`

![](vite-vscode.png)