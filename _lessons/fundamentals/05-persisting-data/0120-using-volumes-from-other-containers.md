---
lesson_id: f72360ec2bce
title: Using volumes from other containers
permalink: "/fundamentals/persisting-data/using-volumes-from-other-containers/"
course: fundamentals
vimeo: '259597846'
type: video
discussion_id: f72360ec2bce
---

## Commands
```sh
docker container run --name c1 --rm --volume /data -it alpine:latest
docker container run --volumes-from c1 -it --rm alpine:latest
```
