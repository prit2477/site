---
lesson_id: 8eb41cad7b03
title: User defined networks and links
permalink: "/fundamentals/networking-101/user-defined-networks-and-links/"
course: fundamentals
vimeo: '259597884'
type: video
discussion_id: 8eb41cad7b03
---

## Commands
```sh
docker container run --network mynet --name postgres --rm -d postgres:9.6.6-alpine
docker container run --network mynet -it --rm --link postgres:pg alpine:latest
ping postgres
ping pg
```
