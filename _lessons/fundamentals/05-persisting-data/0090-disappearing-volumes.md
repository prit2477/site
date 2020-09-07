---
lesson_id: 3f1ca1618f67
title: Disappearing volumes
permalink: "/fundamentals/persisting-data/disappearing-volumes/"
course: fundamentals
vimeo: '259597839'
type: video
discussion_id: 3f1ca1618f67
---

## Commands
```sh
docker container run --rm -v /data alpine:latest echo hello
docker container run --rm -v test-volume:/data alpine:latest echo hello
docker volume ls
```
