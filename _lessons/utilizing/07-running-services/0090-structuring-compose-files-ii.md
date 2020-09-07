---
lesson_id: fab99f188833
title: Structuring Compose files II
permalink: "/utilizing/running-services/structuring-compose-files-ii/"
course: utilizing
vimeo: '259617768'
type: video
discussion_id: fab99f188833
---

## Preparation for the video
* [Change the code to support configuring the number of requests](https://github.com/learndocker/docker_examples/commit/163301a)
* [Split up dev and prod settings for Compose](https://github.com/learndocker/docker_examples/commit/b2f9127)

## Commands
```sh
docker-compose -f docker-compose.yml -f docker-compose.prod.yml config
docker-compose -f docker-compose.yml -f docker-compose.prod.yml config > docker-stack.yml
docker stack deploy -c docker-stack.yml demo
```
