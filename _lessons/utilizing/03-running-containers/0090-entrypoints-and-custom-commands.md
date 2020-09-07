---
lesson_id: 987ed18a61e7
title: Entrypoints and custom commands
permalink: "/utilizing/running-containers/entrypoints-and-custom-commands/"
course: utilizing
vimeo: '259610400'
type: video
discussion_id: 987ed18a61e7
---

## Changes to the examples
* [Handle custom commands for the ENTRYPOINT](https://github.com/learndocker/docker_examples/commit/334b03e)

## Links
* [ENTRYPOINT](https://docs.docker.com/engine/reference/builder/#entrypoint)

## Commands
```sh
docker-compose run nginx
docker-compose run nginx echo 1
docker-compose build
docker-compose run nginx echo 1
docker-compose run nginx nginx -t
docker-compose build
docker-compose up
```
