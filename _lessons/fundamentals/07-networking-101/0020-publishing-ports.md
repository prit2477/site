---
lesson_id: aa584c933c84
title: Publishing ports
permalink: "/fundamentals/networking-101/publishing-ports/"
course: fundamentals
vimeo: '259597865'
type: video
discussion_id: aa584c933c84
---

## Commands
```sh
docker container run --publish 8080:80 -d nginx:latest
docker container ls
docker container run --publish 127.0.0.1:80:80 -d nginx:latest
docker container run -it alpine:latest
ip addr
```
