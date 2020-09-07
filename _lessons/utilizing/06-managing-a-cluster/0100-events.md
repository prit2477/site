---
lesson_id: 82a66d30832f
title: Events
permalink: "/utilizing/managing-a-cluster/events/"
course: utilizing
vimeo: '259616473'
type: video
discussion_id: 82a66d30832f
---

## Links
* [Docker events](https://docs.docker.com/engine/reference/commandline/events/)

## Commands
```sh
docker events
docker service ls
docker service update --replicas 1 demo-frontend
docker events --filter scope=swarm
docker service update --replicas 10 demo-frontend
docker network create --driver overlay foobar
docker events --filter scope=local
docker service update --replicas 1 demo-frontend
docker events --filter scope=local --filter event=container --filter event=destroy
docker events --help
```
