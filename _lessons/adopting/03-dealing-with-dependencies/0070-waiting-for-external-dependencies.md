---
lesson_id: 787cfcc66d1c
title: Waiting for external dependencies
permalink: "/adopting/dealing-with-dependencies/waiting-for-external-dependencies/"
course: adopting
vimeo: '259618225'
type: video
discussion_id: 787cfcc66d1c
---

## Preparation for the video
* [Prepare the Docker related files for the pg_isready example](https://github.com/learndocker/docker_examples/commit/8f87726)

## Changes to the examples
* [Wait for postgres to be up and running via an entrypoint](https://github.com/learndocker/docker_examples/commit/2400560)

## Links
* [Control startup order in Compose](https://docs.docker.com/compose/startup-order/)
* [pg_isready](https://www.postgresql.org/docs/9.6/static/app-pg-isready.html)

## Commands
```sh
docker-compose run app echo 1
```
