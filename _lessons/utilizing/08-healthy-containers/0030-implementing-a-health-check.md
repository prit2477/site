---
lesson_id: ed348cc55dc4
title: Implementing a Health Check
permalink: "/utilizing/healthy-containers/implementing-a-health-check/"
course: utilizing
vimeo: '259617821'
type: video
discussion_id: ed348cc55dc4
---

## Preparation for the video
* [Update the app and add a status endpoint](https://github.com/learndocker/docker_examples/commit/f9994f3)
* [Change the manipulated status endpoint so that it just returns 'ok'](https://github.com/learndocker/docker_examples/commit/1795f09)

## Changes to the examples
* [Add the health check](https://github.com/learndocker/docker_examples/commit/4692ca6)

## Commands
```sh
docker-compose up -d frontend
watch docker container ls
```
