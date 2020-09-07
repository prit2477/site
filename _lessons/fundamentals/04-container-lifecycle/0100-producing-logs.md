---
lesson_id: fa7da59a608a
title: Producing logs
permalink: "/fundamentals/container-lifecycle/producing-logs/"
course: fundamentals
vimeo: '259597808'
type: video
discussion_id: fa7da59a608a
---

## Changes to the examples
* [Add the scripts for the logging demo](https://github.com/learndocker/docker_examples/commit/65e016f)

## Commands
```sh
docker container run -v /Users/julian/workspace/docker_examples/logging_demo/scripts:/app ruby:2.4.2 ruby /app/logger.rb 4350  docker container run -v /Users/julian/workspace/docker_examples/logging_demo/scripts:/app ruby:2.4.2 ruby /app/logger.rb
docker container run -v /Users/julian/workspace/docker_examples/logging_demo/scripts:/app ruby:2.4.2 ruby /app/file-logger.rb 4350  docker container run -v /Users/julian/workspace/docker_examples/logging_demo/scripts:/app ruby:2.4.2 ruby /app/file_logger.rb
```
