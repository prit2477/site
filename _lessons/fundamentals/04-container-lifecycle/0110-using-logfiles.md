---
lesson_id: 19ad1416abec
title: Using logfiles
permalink: "/fundamentals/container-lifecycle/using-logfiles/"
course: fundamentals
vimeo: '259597810'
type: video
discussion_id: 19ad1416abec
---

## Changes to the examples
* [Redirect the access logs to stdout](https://github.com/learndocker/docker_examples/commit/c43fad0)

## Commands
```sh
docker container run --rm --name c1 -p 80:80 jfahrer/nginx:latest
docker container exec c1 tail /var/log/nginx/access.log
docker image build -t jfahrer/nginx:latest .
docker container run --rm --name c1 -p 80:80 jfahrer/nginx:latest
```
