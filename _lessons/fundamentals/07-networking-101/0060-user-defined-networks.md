---
lesson_id: 797e9c4b9ae8
title: User defined networks
permalink: "/fundamentals/networking-101/user-defined-networks/"
course: fundamentals
vimeo: '259597879'
type: video
discussion_id: 797e9c4b9ae8
---

## Links
* https://docs.docker.com/network/

## Commands
```sh
docker network ls
docker network create mynet
docker network ls
docker container run --network mynet --rm -it alpine:latest
docker network rm mynet
```
