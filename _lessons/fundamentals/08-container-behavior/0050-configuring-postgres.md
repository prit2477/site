---
lesson_id: 65661710cb63
title: Configuring postgres
permalink: "/fundamentals/container-behavior/configuring-postgres/"
course: fundamentals
vimeo: '270913175'
type: video
discussion_id: 65661710cb63
---

## Commands
```sh
docker container run --rm --name pg -d -e "POSTGRES_USER=myuser" -e "POSTGRES_PASSWORD=secret" postgres:9.6.6-alpine
docker container run --rm --link pg -it postgres:9.6.6-alpine psql -h pg -U myuser
```
