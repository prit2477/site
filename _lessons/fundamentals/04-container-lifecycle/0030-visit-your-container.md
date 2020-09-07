---
lesson_id: 85de01d45071
title: Visit your container
permalink: "/fundamentals/container-lifecycle/visit-your-container/"
course: fundamentals
vimeo: '259597785'
type: video
discussion_id: 85de01d45071
---

## Commands
```sh
docker container run --name c1 --rm -d nginx:latest
docker container exec c1 cat /etc/nginx/nginx.conf
docker container exec -it c1 sh
```
