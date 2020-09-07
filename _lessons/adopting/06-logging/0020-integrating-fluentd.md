---
lesson_id: 6c34382b0e70
title: Integrating fluentd
permalink: "/adopting/logging/integrating-fluentd/"
course: adopting
vimeo: '259618752'
type: video
discussion_id: 6c34382b0e70
---

## Changes to the examples
* [Add the stack file and config for fluentd](https://github.com/learndocker/docker_examples/commit/80f4ffd)

## Links
* [fluentd](https://www.fluentd.org/)

## Commands
```sh
docker stack deploy -c docker-stack.yml logging
docker stack services logging
docker service logs logging_fluentd
```
