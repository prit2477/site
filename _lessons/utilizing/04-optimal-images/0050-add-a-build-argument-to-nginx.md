---
lesson_id: c2f282de0b87
title: Add a build argument to nginx
permalink: "/utilizing/optimal-images/add-a-build-argument-to-nginx/"
course: utilizing
vimeo: '259610468'
type: assignment
discussion_id: c2f282de0b87
---

## Changes to the examples
* [Add the assignment to intgrate a build arg](https://github.com/learndocker/docker_examples/commit/157854c)

## Changes to complete the assignment
* [Add a build arg for the pkg to the nginx image](https://github.com/learndocker/docker_examples/commit/de35507)

## Links
* [Nginx on Debian](https://wiki.debian.org/Nginx)

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
