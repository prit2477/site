---
lesson_id: ad6308a49798
title: The mount option
permalink: "/fundamentals/persisting-data/the-mount-option/"
course: fundamentals
vimeo: '259597823'
type: video
discussion_id: ad6308a49798
---

## Commands
```sh
docker container run --volume "$(pwd)/html":/usr/share/nginx/html:ro -p 80:80 nginx:latest
docker container run --mount type=bind,src="$(pwd)/html",dst=/usr/share/nginx/html,readonly -p 80:80 nginx:latest
```
