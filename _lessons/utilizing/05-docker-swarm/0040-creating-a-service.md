---
lesson_id: d2a730f5362f
title: Creating a service
permalink: "/utilizing/docker-swarm/creating-a-service/"
course: utilizing
vimeo: '259610651'
type: video
discussion_id: d2a730f5362f
---

## Commands
```sh
docker service create alpine:3.6 tail /dev/null
docker service ls
docker service update priceless_blackwell --replicas 3
docker service ls
```
