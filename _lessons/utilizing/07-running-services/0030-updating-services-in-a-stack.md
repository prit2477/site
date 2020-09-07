---
lesson_id: 4d471f0dc4dd
title: Updating services in a stack
permalink: "/utilizing/running-services/updating-services-in-a-stack/"
course: utilizing
vimeo: '259617182'
type: video
discussion_id: 4d471f0dc4dd
---

## Preparation for the video
* [Display the last 30 instead of 25 requests as v6](https://github.com/learndocker/docker_examples/commit/99c460d)

## Changes to the examples
* [Update the frontend to v6](https://github.com/learndocker/docker_examples/commit/8a7b579)

## Commands
```sh
docker stack services demo
docker stack ps demo
docker stack deploy -c docker-stack.yml demo
```
