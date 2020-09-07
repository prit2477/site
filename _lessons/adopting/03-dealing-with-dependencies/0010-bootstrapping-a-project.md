---
lesson_id: d44370821738
title: Bootstrapping a project
permalink: "/adopting/dealing-with-dependencies/bootstrapping-a-project/"
course: adopting
vimeo: '259618118'
type: video
discussion_id: d44370821738
---

## Changes to the examples
* [Add a Dockerfile to bootstrap a Ruby on Rails project](https://github.com/learndocker/docker_examples/commit/6e44736)

## Commands
```sh
docker image build -t rails .
docker container run rails new foobar
```
