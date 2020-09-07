---
lesson_id: '719859876737'
title: Shortening the command
permalink: "/fundamentals/persisting-data/shortening-the-command/"
course: fundamentals
vimeo: '259597820'
type: video
discussion_id: '719859876737'
---

## Commands
```sh
docker container run -v /Users/julian/workspace/docker_examples/nginx/html:/var/www/html:ro -p 80:80 nginx:latest
docker container run -v "$(pwd)/html":/var/www/html:ro -p 80:80 nginx:latest
```
