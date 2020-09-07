---
lesson_id: ce163d962112
title: Sharing names
permalink: "/fundamentals/networking-101/sharing-names/"
course: fundamentals
vimeo: '259597886'
type: video
discussion_id: ce163d962112
---

## Commands
```sh
docker container run -d --network mynet --network-alias webserver nginx:latest
docker container run -d --network mynet --network-alias webserver nginx:latest
docker container run -d --network mynet --network-alias webserver nginx:latest
docker container run --network mynet -it alpine:latest
nslookup webserver
```
