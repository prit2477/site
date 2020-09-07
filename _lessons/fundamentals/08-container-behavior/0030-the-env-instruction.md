---
lesson_id: bdc49e7c148b
title: The ENV instruction
permalink: "/fundamentals/container-behavior/the-env-instruction/"
course: fundamentals
vimeo: '259597891'
type: video
discussion_id: bdc49e7c148b
---

## Changes to the examples
* [Add the PS1 environment variable](https://github.com/learndocker/docker_examples/commit/08ef86a)
* [Add a second variable to the ENV instruction](https://github.com/learndocker/docker_examples/commit/0c72940)

## Commands
```sh
docker container run jfahrer/myalpine:latest env
docker container run -e "PS2=> " jfahrer/myalpine:latest env
```
