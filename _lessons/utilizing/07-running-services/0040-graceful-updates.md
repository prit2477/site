---
lesson_id: dbbed2820d34
title: Graceful updates
permalink: "/utilizing/running-services/graceful-updates/"
course: utilizing
vimeo: '259617385'
type: video
discussion_id: dbbed2820d34
---

## Preparation for the video
* [Simulate an error for v7](https://github.com/learndocker/docker_examples/commit/7ec818f)

## Changes to the examples
* [Add the update_config key to the Stack file](https://github.com/learndocker/docker_examples/commit/5b102a7)

## Links
* [UPDATE_CONFIG](https://docs.docker.com/compose/compose-file/#update_config)

## Commands
```sh
docker stack deploy -c docker-stack.yml demo
docker stack services demo
docker stack ps demo
docker service logs tsxwjmj2nu4g
```
