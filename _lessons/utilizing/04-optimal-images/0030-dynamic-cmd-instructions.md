---
lesson_id: bf31d9c2d568
title: Dynamic CMD instructions
permalink: "/utilizing/optimal-images/dynamic-cmd-instructions/"
course: utilizing
vimeo: '259610453'
type: video
discussion_id: bf31d9c2d568
---

## Changes to the examples
* [Add a build argument for the default shell](https://github.com/learndocker/docker_examples/commit/a8f8fbd)

## Links
* [Environment replacement](https://docs.docker.com/engine/reference/builder/#environment-replacement)

## Commands
```
docker image build -t jfahrer/myalpine:latest --build-arg MYSHELL=zsh .
docker container run -it jfahrer/myalpine:latest
ps
```
