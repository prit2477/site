---
lesson_id: debd91fa82c1
title: Command line containers
permalink: "/utilizing/running-containers/command-line-containers/"
course: utilizing
vimeo: '259610407'
type: video
discussion_id: debd91fa82c1
---

## Changes to the examples
* [Add the files for the cli example](https://github.com/learndocker/docker_examples/commit/a99d262)
* [Add a default command via a CMD instruction](https://github.com/learndocker/docker_examples/commit/1127401)

## Links
* [ENTRYPOINT](https://docs.docker.com/engine/reference/builder/#entrypoint)

## Commands
```sh
docker-compose build
docker container run jfahrer/curl www.docker.com
docker-compose build
docker container run jfahrer/curl www.docker.com
```
