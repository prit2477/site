---
lesson_id: 181063d07dcf
title: Debugging the issue from the last assignment
permalink: "/fundamentals/container-lifecycle/debugging-the-issue-from-the-last-assignment/"
course: fundamentals
vimeo: '259597795'
type: video
discussion_id: 181063d07dcf
---

## Changes to the examples
* [Add the initial nginx Dockerfile](https://github.com/learndocker/docker_examples/commit/db9cadf)

## The initial Dockerfile
```Dockerfile
FROM debian:buster-slim

RUN apt-get update
RUN apt-get install -y nginx

CMD nginx -g 'daemon off;'
```

## Commands
```sh
docker image build -t jfahrer/nginx:latest . && docker container run --name c1 --rm jfahrer/nginx:latest
docker container exec -it c1 bash
apt-get update && apt-get install procps
ps -ef
```
