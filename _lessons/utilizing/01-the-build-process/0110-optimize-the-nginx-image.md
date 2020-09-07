---
lesson_id: ea582bf46048
title: Optimize the nginx image
permalink: "/utilizing/the-build-process/optimize-the-nginx-image/"
course: utilizing
vimeo: '259610176'
type: assignment
discussion_id: ea582bf46048
---

## Changes to the examples
* [Add the assignment to optimize the nginx Dockerfile](https://github.com/learndocker/docker_examples/commit/dbcbca1)

## The Dockerfile
```
FROM debian:buster-slim

RUN apt-get update
RUN apt-get install -y nginx
RUN rm /var/log/nginx/access.log && ln -s /dev/stdout /var/log/nginx/access.log
RUN rm /var/log/nginx/error.log && ln -s /dev/stderr /var/log/nginx/error.log

COPY ./html/ /var/www/html/
ADD http://example.com/index.html /var/www/html/example.html

CMD ["/usr/sbin/nginx", "-g", "daemon off;"]
```
