---
lesson_id: c22b6e5b726b
title: Verify it is PID1
permalink: "/fundamentals/container-lifecycle/verify-it-is-pid1/"
course: fundamentals
vimeo: '259597800'
type: assingment
discussion_id: c22b6e5b726b
---

## The Dockerfile
```
FROM debian:buster-slim

RUN apt-get update
RUN apt-get install -y nginx

CMD ["/usr/sbin/nginx", "-g", "daemon off;"]
```
