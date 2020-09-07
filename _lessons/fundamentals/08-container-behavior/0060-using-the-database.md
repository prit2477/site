---
lesson_id: 9da43e12fa78
title: Using the database
permalink: "/fundamentals/container-behavior/using-the-database/"
course: fundamentals
vimeo: '259609811'
type: video
discussion_id: 9da43e12fa78
---

## Changes to the examples
* [Add the example env files for the web app demo](https://github.com/learndocker/docker_examples/commit/4722202)

## The images
* [jfahrer/demo_web_app](https://store.docker.com/community/images/jfahrer/demo_web_app)
* [postgres](https://store.docker.com/images/postgres)

## The commands
```
docker container run -d --name pg --env-file db.env postgres:9.6.6-alpine
docker container run -d --link pg --env-file app.env -p 9292:9292 jfahrer/demo_web_app
```
