---
lesson_id: 63ee18a035e6
title: Naming volumes
permalink: "/fundamentals/persisting-data/naming-volumes/"
course: fundamentals
vimeo: '259597831'
type: video
discussion_id: 63ee18a035e6
---

## Commands
```sh
docker container run -it --volume my-volume:/data alpine:latest
touch /data/test.file
docker volume ls
docker container run -it --volume my-volume:/data alpine:latest
ls -l /data
docker container rm -f $(docker container ls -aq) # BEWARE - This command will delete ALL containers on the system
docker container ls -a
docker volume ls
```
