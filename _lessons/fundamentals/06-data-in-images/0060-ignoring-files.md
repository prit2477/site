---
lesson_id: c374811ad7ed
title: Ignoring files
permalink: "/fundamentals/data-in-images/ignoring-files/"
course: fundamentals
vimeo: '259597860'
type: video
discussion_id: c374811ad7ed
---

## Changes to the examples
* [Add the Dockerfile and .dockerignore file](https://github.com/learndocker/docker_examples/commit/adf6c39)

## Links
* [The .dockerignore file](https://docs.docker.com/engine/reference/builder/#dockerignore-file)

## Commands
```sh
docker image build .
ls -l data/
du -sh data/*
echo data/tmp >> .dockerignore
docker image build .
```
