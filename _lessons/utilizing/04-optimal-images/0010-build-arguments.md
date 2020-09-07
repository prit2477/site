---
lesson_id: de2a989cd7db
title: Build arguments
permalink: "/utilizing/optimal-images/build-arguments/"
course: utilizing
vimeo: '259610434'
type: video
discussion_id: de2a989cd7db
---

## Changes to the examples
* [Add the script and initial Dockerfile for the greeter](https://github.com/learndocker/docker_examples/commit/6b86450)
* [Add the build argument to the Dockerfile](https://github.com/learndocker/docker_examples/commit/775e2ce)

## Commands
```sh
docker container run jfahrer/greeter:latest
docker container run -e NAME=Julian jfahrer/greeter:latest

docker image build -t jfahrer/greeter:lateast .
docker container run jfahrer/greeter:latest

docker image build -t jfahrer/greeter:lateast --build-arg NAME=Julian .
docker container run jfahrer/greeter:latest
docker container run -e NAME=World jfahrer/greeter:latest
```
