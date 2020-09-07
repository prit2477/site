---
lesson_id: 5506c5c48fc5
title: Reading logs
permalink: "/fundamentals/container-lifecycle/reading-logs/"
course: fundamentals
vimeo: '259597803'
type: video
discussion_id: 5506c5c48fc5
---

## Commands
```sh
docker container run --rm --name c1 -p 80:80 nginx:latest
curl localhost
docker container run --rm --name c1 -p 80:80 -d nginx:latest
curl localhost
docker container logs c1
docker container logs -f c1
curl localhost
```
