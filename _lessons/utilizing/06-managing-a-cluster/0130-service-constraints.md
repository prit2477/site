---
lesson_id: 0df43abb87b6
title: Service Constraints
permalink: "/utilizing/managing-a-cluster/service-constraints/"
course: utilizing
vimeo: '259616492'
type: video
discussion_id: 0df43abb87b6
---

## Links
* [Specify service constraints](https://docs.docker.com/engine/reference/commandline/service_create/#specify-service-constraints-constraint)

## Commands
```sh
docker service create --constraint node.hostname==node3 --name stable alpine:3.6 tail -f /dev/null
docker service ls
docker service ps stable
docker service update --replicas 10 stable
docker service ps stable
```
