---
lesson_id: 84e0ec05c6d2
title: Extracting data from containers
permalink: "/adopting/dealing-with-dependencies/extracting-data-from-containers/"
course: adopting
vimeo: '259618136'
type: video
discussion_id: 84e0ec05c6d2
---

## Changes to the examples
* [Add the Gemfile.lock](https://github.com/learndocker/docker_examples/commit/114296a)

## Commands
```sh
docker-compose build
docker container run --name c1 jfahrer/webapp-ruby:latest echo 1
docker container cp c1:/app/Gemfile.lock .
```
