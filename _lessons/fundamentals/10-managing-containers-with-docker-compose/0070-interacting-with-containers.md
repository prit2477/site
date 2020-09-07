---
lesson_id: 5a8eee10069a
title: Interacting with containers
permalink: "/fundamentals/managing-containers-with-docker-compose/interacting-with-containers/"
course: fundamentals
vimeo: '259620640'
type: video
discussion_id: 5a8eee10069a
---

## Changes to the examples
* [Add the alpine service to the compose file](https://github.com/learndocker/docker_examples/commit/7f5322f)

## Commands
```sh
docker-compose up -d
docker-compose exec alpine sh
ping composeexample_pg_1
ping pg
exit
docker-compose stop alpine
docker-compose rm alpine
docker-compose up -d
```
