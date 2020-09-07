---
lesson_id: 608d12517eb6
title: Updating a service
permalink: "/utilizing/docker-swarm/updating-a-service/"
course: utilizing
vimeo: '259610685'
type: video
discussion_id: 608d12517eb6
---

## Preparation for the video
* [Change the bg color to grey for v2](https://github.com/learndocker/docker_examples/commit/913ee36)

## Commands
```sh
docker service update --image jfahrer/swarm-demo-frontend:v2 publish-demo
docker service ps publish-demo
```
