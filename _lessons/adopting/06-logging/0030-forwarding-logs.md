---
lesson_id: 9b9e4d8f5711
title: Forwarding logs
permalink: "/adopting/logging/forwarding-logs/"
course: adopting
vimeo: '259618768'
type: video
discussion_id: 9b9e4d8f5711
---

## Changes to the examples
* [Add the client service](https://github.com/learndocker/docker_examples/commit/4bf9379)
* [Set the logging driver for the client service](https://github.com/learndocker/docker_examples/commit/d876384)

## Commands
```sh
docker stack deploy -c docker-stack.yml logging
docker service logs -f logging_client
docker service logs -f logging_fluentd
```
