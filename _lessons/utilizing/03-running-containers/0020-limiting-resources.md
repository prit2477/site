---
lesson_id: c05c82cc83c2
title: Limiting resources
permalink: "/utilizing/running-containers/limiting-resources/"
course: utilizing
vimeo: '259610335'
type: video
discussion_id: c05c82cc83c2
---

## Links
* [Limit a container's resources](https://docs.docker.com/config/containers/resource_constraints/)

## Commands
```sh
docker container run -d --memory 256M --cpus 0.25 alpine:latest
docker container run -d --memory-reservation 256M --cpu-shares 1024 alpine:latest
```
