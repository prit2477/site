---
lesson_id: 384d40e6e4e6
title: More on env vars
permalink: "/fundamentals/container-behavior/more-on-env-vars/"
course: fundamentals
vimeo: '270913162'
type: video
discussion_id: 384d40e6e4e6
---

## Commands
```sh
docker container run alpine:latest env
echo MYVAR=test >> app.env
echo FOO=bar >> app.env
docker container run alpine:latest env
export OTHERVAR=local-test
docker container run --env-file app.env -e OTHERVAR alpine:latest env
echo OTHERVAR >> app.env
docker container run --env-file app.env alpine:latest env
```
