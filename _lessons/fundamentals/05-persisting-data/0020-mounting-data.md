---
lesson_id: dbbee07475e7
title: Mounting data
permalink: "/fundamentals/persisting-data/mounting-data/"
course: fundamentals
vimeo: '259597818'
type: video
discussion_id: dbbee07475e7
---

## Commands
```sh
docker container run --volume /Users/julian/workspace/docker_examples/nginx/html:/var/www/html:ro -p 80:80 jfahrer/nginx:latest
```
