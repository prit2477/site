---
lesson_id: 60f29fdc993a
title: Secrets with Docker Stack
permalink: "/utilizing/running-services/secrets-with-docker-stack/"
course: utilizing
vimeo: '259617473'
type: video
discussion_id: 60f29fdc993a
---

## Preparation for the video
* [Use a secrets file for the postgres password](https://github.com/learndocker/docker_examples/commit/65b561f)

## Changes to the examples
* [Use a secret for the postgres password](https://github.com/learndocker/docker_examples/commit/445ed20)

## Links
* [Manage sensitive data with Docker secrets](https://docs.docker.com/engine/swarm/secrets/)
* [secrets configuration reference](https://docs.docker.com/compose/compose-file/#secrets-configuration-reference)


## Commands
```sh
echo 'secret' | docker secret create pg_secret -
docker secret ls
docker stack deploy -c docker-stack.yml demo
``
