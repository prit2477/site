---
lesson_id: 786d4353349f
title: Integrate the demo_web_app
permalink: "/fundamentals/managing-containers-with-docker-compose/integrate-the-demo_web_app/"
course: fundamentals
vimeo: '259609982'
type: assignment
discussion_id: 786d4353349f
---

## Changes to the examples
* [Add the assignment](https://github.com/learndocker/docker_examples/commit/bd9f0c0)

## Images
* [jfahrer/demo_web_app](https://store.docker.com/community/images/jfahrer/demo_web_app)
* [postgres](https://store.docker.com/images/postgres)

## The files
* db.env
  ```
  POSTGRES_DB=web_app_db
  POSTGRES_USER=app
  POSTGRES_PASSWORD=secret
  ```

* docker-compose.yml
  ```
  version: '3.3'

  services:
    web:
      image: nginx:latest
      ports:
        - 80:80
      volumes:
        - ./html:/usr/share/nginx/html

    pg:
      image: postgres:9.6-alpine
      env_file:
        - ./db.env
      volumes:
        - pg-data:/var/lib/postgresql/data

    alpine:
      image: alpine:latest
      stdin_open: true
      tty: true
      command: sh

  volumes:
    pg-data:
  ```
