---
lesson_id: e6a15a67fcc4
title: Resolving hostnames
permalink: "/fundamentals/networking-101/resolving-hostnames/"
course: fundamentals
vimeo: '259597882'
type: video
discussion_id: e6a15a67fcc4
---

## Commands
```sh
docker container run --network mynet --name c1 --rm -it alpine:latest
docker container run --network mynet --name c2 --rm -it alpine:latest
docker container run --network mynet --name c2 --rm -it --ip 172.18.0.99 alpine:latest
```
