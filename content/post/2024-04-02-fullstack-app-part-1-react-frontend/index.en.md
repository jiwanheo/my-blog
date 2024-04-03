---
title: 'Fullstack app [Part 1]: React frontend'
author: Jiwan Heo
date: '2024-04-02'
DisableComments: no
---

In this post, we'll make a very simple react app that interacts with a database.
This app will let users bookmark websites. Users will be able to see the latest
bookmark, and on request, a complete list of all bookmarks.

So this is 1 POST request, and 2 GET requests - one for seeing the latest 
bookmark, and another to query n number of bookmarks (maybe this can be one, 
with parameter).