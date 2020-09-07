---
lesson_id: 7ca795e268e8
title: Replication mode
permalink: "/utilizing/running-services/replication-mode/"
course: utilizing
vimeo: '259617783'
type: video
discussion_id: 7ca795e268e8
---

## Changes to the examples
* [Set the mode for the lb service to global](https://github.com/learndocker/docker_examples/commit/a857513)

## Commands
```sh
docker-compose -f docker-compose.yml -f docker-compose.prod.yml config > docker-stack.yml
docker stack deploy -c docker-stack.yml demo
docker service ls
docker service ps demo_lb
```
