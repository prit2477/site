---
lesson_id: fe270e7659a4
title: Setting up a demo
permalink: "/utilizing/managing-a-cluster/setting-up-a-demo/"
course: utilizing
vimeo: '259616749'
type: assignment
discussion_id: fe270e7659a4
---

## Preparation for the video
* [Add the src code for the swarm-demo-db service](https://github.com/learndocker/docker_examples/commit/3e8836d)
* [Update the swarm-demo-frontend to v5](https://github.com/learndocker/docker_examples/commit/c66df67)

## Changes to the examples
* [Add the assignment to create the demo services](https://github.com/learndocker/docker_examples/commit/4a1d5b7)

## Environment variables
```sh
POSTGRES_USER=demo
POSTGRES_PASSWORD=secret
POSTGRES_DB=demo
POSTGRES_HOST=demo-db
PROXY_UPSTREAM=demo-frontend:8080
```

## Images
* [jfahrer/swarm-demo-frontend](https://store.docker.com/community/images/jfahrer/swarm-demo-frontend)
* [jfahrer/swarm-demo-db](https://store.docker.com/community/images/jfahrer/swarm-demo-db)
* [jfahrer/swarm-demo-lb](https://store.docker.com/community/images/jfahrer/swarm-demo-lb)
