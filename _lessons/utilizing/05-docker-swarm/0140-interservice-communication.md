---
lesson_id: 500aa7a699b8
title: Interservice communication
permalink: "/utilizing/docker-swarm/interservice-communication/"
course: utilizing
vimeo: '259610735'
type: video
discussion_id: 500aa7a699b8
---

## Commands
```sh
docker network create --driver overlay service-net
docker service create --name service1 --network service-net alpine:3.6 ping service2
docker service ls
docker service create --name service2 --network service-net alpine:3.6 tail -f /dev/null
docker service logs service1
```
