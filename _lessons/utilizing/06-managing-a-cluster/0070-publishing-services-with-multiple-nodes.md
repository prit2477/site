---
lesson_id: 41cbbbe9d033
title: Publishing services with multiple nodes
permalink: "/utilizing/managing-a-cluster/publishing-services-with-multiple-nodes/"
course: utilizing
vimeo: '259616246'
type: video
discussion_id: 41cbbbe9d033
---

## Commands
```sh
docker service create --name demo-frontend --publish 8080:8080 jfahrer/swarm-demo-frontend:v1
docker service ps demo-frontend
```
