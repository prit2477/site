---
lesson_id: e8c75fcabbf8
title: Labels
permalink: "/adopting/swarm-in-production/labels/"
course: adopting
vimeo: '259618061'
type: video
discussion_id: e8c75fcabbf8
---

## Preparation for the video
* [Prepare the stack file for the labels example](https://github.com/learndocker/docker_examples/commit/57eac23)

## Changes to the examples
* [Make use of labels in the stack file](https://github.com/learndocker/docker_examples/commit/ee35bd1)

## Links
* [Docker object labels](https://docs.docker.com/config/labels-custom-metadata/)

## Commands
```sh
docker node ls
docker node update --label-add region=us-west1
docker stack deploy -c docker-stack.yml demo
docker service ps filter desired-state=running demo_frontend
docker container ls --filter label=app=demo
```
