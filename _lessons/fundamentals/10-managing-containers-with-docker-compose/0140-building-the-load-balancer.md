---
lesson_id: 1cb3fa562b2d
title: Building the load balancer
permalink: "/fundamentals/managing-containers-with-docker-compose/building-the-load-balancer/"
course: fundamentals
vimeo: '259610038'
type: video
discussion_id: 1cb3fa562b2d
---

## Changes to the examples
* [Add the PROXY_UPSTREAM env var to the .env file](https://github.com/learndocker/docker_examples/commit/06f4733)
* [Remove the web service definition and stop publishing the webapp](https://github.com/learndocker/docker_examples/commit/1d8ddbc)
* [Add the service definition for the load balancer](https://github.com/learndocker/docker_examples/commit/5c4f051)
* [Add the build directive to the load balancer service](https://github.com/learndocker/docker_examples/commit/ebbe37b)

## Commands
```sh
docker-compose build
docker-compose build lb
docker-compose up --build
```
