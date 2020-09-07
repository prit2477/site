---
lesson_id: 59973c6d65e1
title: Leightweight images
permalink: "/utilizing/the-build-process/leightweight-images/"
course: utilizing
vimeo: '259610122'
type: video
discussion_id: 59973c6d65e1
---

## Changes to the examples
* [Add a RUN instruction to delete temporary files](https://github.com/learndocker/docker_examples/commit/6e71b1b)
* [Chain the commands to a single RUN instruction](https://github.com/learndocker/docker_examples/commit/efadaac)

## Commands
```sh
docker image ls jfahrer/myalpine:latest
docker image build -t jfahrer/myalpine:latest .
docker image ls jfahrer/myalpine:latest
```
