---
lesson_id: dfc02c122e06
title: The build process
permalink: "/utilizing/the-build-process/the-build-process/"
course: utilizing
vimeo: '259610076'
type: video
discussion_id: dfc02c122e06
---

## Links
* [Create a new image from a container’s changes](https://docs.docker.com/engine/reference/commandline/container_commit/)

## Commands
```sh
docker image build -t jfahrer/myalpine:latest .
docker image history jfahrer/myalpine:latest
docker image build -t jfahrer/myalpine:latest --no-cache .
```
