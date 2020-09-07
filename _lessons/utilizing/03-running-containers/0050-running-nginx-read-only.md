---
lesson_id: d8b6ba92fa7e
title: Running nginx read-only
permalink: "/utilizing/running-containers/running-nginx-read-only/"
course: utilizing
vimeo: '259610363'
type: assignment
discussion_id: d8b6ba92fa7e
---

## Changes to the examples
* [Add the assigment to run nginx read only](https://github.com/learndocker/docker_examples/commit/25cae6a)
* [Update the Dockerfile for the assignment](https://github.com/learndocker/docker_examples/commit/33d2958)

## The Dockerfile
```
FROM debian:buster-slim

RUN apt-get update \
      && apt-get install -y nginx \
      && rm /var/log/nginx/access.log \
      && rm /var/log/nginx/error.log \
      && ln -s /dev/stdout /var/log/nginx/access.log \
      && ln -s /dev/stderr /var/log/nginx/error.log

CMD ["/usr/sbin/nginx", "-g", "daemon off;"]
```
