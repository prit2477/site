---
lesson_id: bb5ac616c90a
title: Using a volume
permalink: "/fundamentals/managing-containers-with-docker-compose/using-a-volume/"
course: fundamentals
vimeo: '259609976'
type: video
discussion_id: bb5ac616c90a
---

## Changes to the examples
* [Add a named volume to the pg service](https://github.com/learndocker/docker_examples/commit/3168e07)

## Commands
```sh
vim docker-compose.yml
docker-compose up -d pg
docker-compose down
docker volume ls
```
