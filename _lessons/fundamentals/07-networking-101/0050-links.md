---
lesson_id: edd88d4ccfea
title: Links
permalink: "/fundamentals/networking-101/links/"
course: fundamentals
vimeo: '259597876'
type: video
discussion_id: edd88d4ccfea
---

## Commands
```sh
docker container run --name webserver --rm -d nginx:latest
docker container run --link webserver -it alpine:latest
docker container run --link webserver:ws -it alpine:latest
```
