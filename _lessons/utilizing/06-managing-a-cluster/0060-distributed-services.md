---
lesson_id: 3c52892dd95c
title: Distributed services
permalink: "/utilizing/managing-a-cluster/distributed-services/"
course: utilizing
vimeo: '259616233'
type: video
discussion_id: 3c52892dd95c
---

## Commands
```sh
docker node ls
docker service create --name demo alpine:3.6 tail -f /dev/null
docker service ls
docker service ps demo
docker service update --replicas 10 demo
```
