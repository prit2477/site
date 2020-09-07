---
lesson_id: 380d4fab41b6
title: Dealing with volumes
permalink: "/utilizing/managing-a-cluster/dealing-with-volumes/"
course: utilizing
vimeo: '259616484'
type: video
discussion_id: 380d4fab41b6
---

## Commands
```sh
docker node ls
docker service create --name test --mount src=volume1,dst=/data,type=volume alpine:3.6 tail -f /dev/null
docker service ps test
docker volume ls
```
