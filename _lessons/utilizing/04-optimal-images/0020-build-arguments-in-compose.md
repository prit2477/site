---
lesson_id: d53b23c71206
title: Build arguments in Compose
permalink: "/utilizing/optimal-images/build-arguments-in-compose/"
course: utilizing
vimeo: '259610443'
type: video
discussion_id: d53b23c71206
---

## Changes to the examples
* [Add the inital docker-compose.yml](https://github.com/learndocker/docker_examples/commit/ba6202c)
* [Add the args directive to the docker-compose.yml](https://github.com/learndocker/docker_examples/commit/15e198c)

## Commands
```sh
docker-compose build
docker-compose run app
docker-compose build --build-arg NAME=Jeffrey app
docker-compose run app
```
