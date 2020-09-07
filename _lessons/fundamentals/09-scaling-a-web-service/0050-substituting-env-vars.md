---
lesson_id: d9ed9a0caa17
title: Substituting ENV vars
permalink: "/fundamentals/scaling-a-web-service/substituting-env-vars/"
course: fundamentals
vimeo: '259609875'
type: video
discussion_id: d9ed9a0caa17
---

## Changes to the examples
* [Add the files for the jfahrer/envsubst image](https://github.com/learndocker/docker_examples/commit/1a675ed)

## Commands
```sh
docker container run -it jfahrer/lb:latest bash
cat example_file
export VAR1='test' OTHER='some text'
envsubst < example_file
envsubst '$OTHER' < example_file
envsubst '$OTHER' < example_file > example_file.new
cat example_file.new
```
