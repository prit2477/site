---
lesson_id: a314b87cfa7a
title: Cleaning things up
permalink: "/fundamentals/getting-started/cleaning-things-up/"
course: fundamentals
vimeo: '259597723'
type: video
discussion_id: a314b87cfa7a
---

## Commands
```sh
docker container ls -a
docker container rm d610b552c56e
docker container ls -aq
docker container rm $(docker container ls -aq)
docker image ls
docker image rm hello-world
```
