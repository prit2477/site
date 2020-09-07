---
lesson_id: 173c29c814b9
title: Using a tmpfs
permalink: "/utilizing/running-containers/using-a-tmpfs/"
course: utilizing
vimeo: '259610353'
type: video
discussion_id: 173c29c814b9
---

## Commands
```sh
docker container run --tmpfs /tmp -it alpine:latest
docker container run --mount type=tmpfs,dst=/tmp -it alpine:latest
docker container run --mount type=tmpfs,dst=/tmp --read-only -it alpine:latest
```
