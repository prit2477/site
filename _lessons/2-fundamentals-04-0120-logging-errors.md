---
title: Logging errors
course: fundamentals
chapter_number: 04
chapter: Container lifecycle
lesson_number: 0120
lesson_id: 4d71e0b1d40d
video_url: https://vimeo.com/259597811
type: video
discussion_id: 4d71e0b1d40d
---
# Changes to the examples
* [Add the 2nd assignment](https://github.com/learndocker/docker_examples/commit/93492dc)

# Resources
## The Dockerfile
```
FROM debian:buster-slim

RUN apt-get update
RUN apt-get install -y nginx
RUN rm /var/log/nginx/access.log && ln -s /dev/stdout /var/log/nginx/access.log

CMD ["/usr/sbin/nginx", "-g", "daemon off;"]
```
