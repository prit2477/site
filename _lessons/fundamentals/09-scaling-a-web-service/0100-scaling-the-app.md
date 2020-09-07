---
lesson_id: b1914ba49eb8
title: Scaling the app
permalink: "/fundamentals/scaling-a-web-service/scaling-the-app/"
course: fundamentals
vimeo: '259609926'
type: assignment
discussion_id: b1914ba49eb8
---

## Changes to the examples
* [Add the assignment](https://github.com/learndocker/docker_examples/commit/0605e1d)

## Images
* [postgres](https://store.docker.com/images/postgres)
* [jfahrer/demo_web_app](https://store.docker.com/community/images/jfahrer/demo_web_app)

## Steps for the previous assignment
* File db.env
  ```sh
  POSTGRES_DB=web_app_db
  POSTGRES_USER=app
  POSTGRES_PASSWORD=secret
  ```

* File app.env
  ```sh
  POSTGRES_DB=web_app_db
  POSTGRES_USER=app
  POSTGRES_PASSWORD=secret
  POSTGRES_HOST=pg
  ```

## Commands
```sh
docker network create mynet
docker container run --network mynet --env-file db.env -v pgdata:/var/lib/postgresql/data -d --name pg postgres:9.6.6-alpine
docker container run --network mynet --env-file app.env -d --name webapp jfahrer/demo_web_app:latest
docker container run --network mynet -e PROXY_UPSTREAM=webapp:9292 -d -p 80:80 --name lb jfahrer/lb:latest
```
