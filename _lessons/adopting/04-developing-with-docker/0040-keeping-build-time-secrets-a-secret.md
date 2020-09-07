---
lesson_id: fb2a2547d193
title: Keeping build time secrets a secret
permalink: "/adopting/developing-with-docker/keeping-build-time-secrets-a-secret/"
course: adopting
vimeo: '259618260'
type: video
discussion_id: fb2a2547d193
---

## Changes to the examples
* [Add the initial Dockerfile for the build time secrets example](https://github.com/learndocker/docker_examples/commit/b2d578b)
* [Introduce a second build stage](https://github.com/learndocker/docker_examples/commit/887b8d7)

## Commands
```sh
docker image build -t test .
docker image build -t test --buld-arg GITHUB_TOKEN=abc .
docker image history test
docker image build -t test --buld-arg GITHUB_TOKEN=abc .
docker image history test
```
