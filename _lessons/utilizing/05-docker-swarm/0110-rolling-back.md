---
lesson_id: 0ee3a536c807
title: Rolling back
permalink: "/utilizing/docker-swarm/rolling-back/"
course: utilizing
vimeo: '259610698'
type: video
discussion_id: 0ee3a536c807
---

## Preparation for the video
* [Simulate a bug for version3](https://github.com/learndocker/docker_examples/commit/d046865)

## Commands
```sh
docker service ls
docker service update --image jfahrer/swarm-demo-frontend:v3 publish-demo
docker service ls
docker service ps publish-demo
docker service rollback publish-demo
```
