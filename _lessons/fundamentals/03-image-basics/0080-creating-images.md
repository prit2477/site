---
lesson_id: ef94f7bf8b25
title: Creating Images
permalink: "/fundamentals/image-basics/creating-images/"
course: fundamentals
vimeo: '259597766'
type: video
discussion_id: ef94f7bf8b25
---

## Changes to the examples
* [Add the initial Dockerfile for the myalpine image](https://github.com/learndocker/docker_examples/commit/84cab07)

## Commands
```sh
docker image build -t myalpine:latest .
docker container run -it myalpine:latest
```
