---
lesson_id: f2ff7d7314fb
title: Controlling the update
permalink: "/utilizing/docker-swarm/controlling-the-update/"
course: utilizing
vimeo: '259610694'
type: video
discussion_id: f2ff7d7314fb
---

## Commands
```sh
docker service update --help
docker service update --update-parallelism 2 --update-order start-first --image jfahrer/swarm-demo-frontend:v1 publish-demo
watch docker service ps publish-demo
```
