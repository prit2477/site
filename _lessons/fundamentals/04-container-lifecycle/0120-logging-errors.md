---
lesson_id: 4d71e0b1d40d
title: Logging errors
permalink: "/fundamentals/container-lifecycle/logging-errors/"
course: fundamentals
vimeo: '259597811'
type: assignment
discussion_id: 4d71e0b1d40d
---

## Changes to the examples
* [Add the 2nd assignment](https://github.com/learndocker/docker_examples/commit/93492dc)

## The Dockerfile
```
FROM debian:buster-slim

RUN apt-get update
RUN apt-get install -y nginx
RUN rm /var/log/nginx/access.log && ln -s /dev/stdout /var/log/nginx/access.log

CMD ["/usr/sbin/nginx", "-g", "daemon off;"]
```
