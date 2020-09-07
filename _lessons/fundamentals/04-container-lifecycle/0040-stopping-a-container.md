---
lesson_id: fe9e05d2c115
title: Stopping a container
permalink: "/fundamentals/container-lifecycle/stopping-a-container/"
course: fundamentals
vimeo: '259597790'
type: video
discussion_id: fe9e05d2c115
---

## Changes to the examples
* [Add the initial Dockerfile for the stop_demo](https://github.com/learndocker/docker_examples/commit/39d19a0)

## Commands
```sh
docker container run --name c1 nginx:latest
docker container stop c1
docker container ls -a
docker container run --name c2 jfahrer/stop_demo:latest
docker container stop c2
docker container run --name c3 jfahrer/stop_demo:latest
docker container kill c3
docker container kill --help
```
