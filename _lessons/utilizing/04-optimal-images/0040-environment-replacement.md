---
lesson_id: 8d6d99440888
title: Environment replacement
permalink: "/utilizing/optimal-images/environment-replacement/"
course: utilizing
vimeo: '259610462'
type: video
discussion_id: 8d6d99440888
---

## Changes to the examples
* [Add the env vars and build args to the Dockerfile](https://github.com/learndocker/docker_examples/commit/adeaf8b)
* [Add the Compose file to build the images](https://github.com/learndocker/docker_examples/commit/87f2d39)

## Links
* [Environment replacement](https://docs.docker.com/engine/reference/builder/#environment-replacement)

## Commands
```
docker-compose build
docker-compose run bash env
docker-compose run zsh env
```
