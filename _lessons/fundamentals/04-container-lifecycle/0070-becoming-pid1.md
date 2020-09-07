---
lesson_id: 39f59d255af4
title: Becoming PID1
permalink: "/fundamentals/container-lifecycle/becoming-pid1/"
course: fundamentals
vimeo: '259597797'
type: video
discussion_id: 39f59d255af4
---

## Changes to the examples
* [Make sure that nginx becomes PID1](https://github.com/learndocker/docker_examples/commit/f01a6bd)

## Links
* [The CMD instruction](https://docs.docker.com/engine/reference/builder/#cmd)

## Commands
```sh
docker image build -t jfahrer/nginx:latest . && docker container run --rm jfahrer/nginx:latest
```
