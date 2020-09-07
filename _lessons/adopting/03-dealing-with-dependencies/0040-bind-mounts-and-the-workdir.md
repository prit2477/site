---
lesson_id: e55786104edc
title: Bind mounts and the workdir
permalink: "/adopting/dealing-with-dependencies/bind-mounts-and-the-workdir/"
course: adopting
vimeo: '259618144'
type: video
discussion_id: e55786104edc
---

## Commands
```sh
docker container run -v $(pwd):/app -w /app ruby:2.4.2 bundle install
```
