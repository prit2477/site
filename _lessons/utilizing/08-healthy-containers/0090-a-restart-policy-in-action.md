---
lesson_id: 5ff31036794d
title: A restart policy in action
permalink: "/utilizing/healthy-containers/a-restart-policy-in-action/"
course: utilizing
vimeo: '259617954'
type: video
discussion_id: 5ff31036794d
---

## Changes to the examples
* [Add the restart policy to frontend service](https://github.com/learndocker/docker_examples/commit/6bde50c)

## Commands
```sh
docker service rm demo_frontend
docker stack deploy -c docker-stack.yml demo
watch docker service ps demo_frontend
```
