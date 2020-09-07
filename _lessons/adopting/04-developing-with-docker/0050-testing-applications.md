---
lesson_id: 6eadd6cad050
title: Testing applications
permalink: "/adopting/developing-with-docker/testing-applications/"
course: adopting
vimeo: '259618306'
type: video
discussion_id: 6eadd6cad050
---

## Changes to the examples
* [Add the example application for the lesson about running tests](https://github.com/learndocker/docker_examples/commit/adbe6f0)

## Commands
```sh
docker-compose run app rspec
docker-compose run --rm app rspec
docker-compose up -d app
docker-compose exec app rspec
```
