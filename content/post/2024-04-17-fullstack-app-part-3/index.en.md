---
title: 'Fullstack App [Part 3]: Container'
author: Jiwan Heo
date: '2024-04-17'
slug: fullstack-app-part-3
DisableComments: no
draft: true
---

In the compose.yaml, we can specify the default root user creds, through 
environment variables.

Also, we can specify some sql commands to run (create db, create role,...) by
writing a .sql file, and attaching it as volumes under compose.yaml. However, 
this .sql file will only run, when there's no existing db. So this means, we 
have to clear the volume when we compose down, via `docker-compose down --volumes`.
When postgres server is running (via `docker-compose up --build`), we can access
psql instance inside the container, by running in the terminal 
`docker exec -it process_id bash`.

And in pool, I have to change 'host' argument, to whatever i named the psql
section in compose.yaml