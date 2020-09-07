---
lesson_id: d1958345c110
title: Using mount for volumes
permalink: "/fundamentals/persisting-data/using-mount-for-volumes/"
course: fundamentals
vimeo: '259597835'
type: video
discussion_id: d1958345c110
---

## Commands
```sh
docker container run -it --mount destination=/data alpine:latest
docker container run -it --mount src=my-volume,destination=/data alpine:latest
docker container run -it --mount src=my-volume,destination=/data,readonly alpine:latest
docker container run -it --mount destination=/data alpine:latest
docker container run -it --mount dst=/data alpine:latest
```
