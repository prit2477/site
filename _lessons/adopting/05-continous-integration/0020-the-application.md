---
lesson_id: 28500babc311
title: The application
permalink: "/adopting/continous-integration/the-application/"
course: adopting
vimeo: '259618411'
type: video
discussion_id: 28500babc311
---

## Changes to the examples
* [Add the source code for the demo application](https://github.com/learndocker/demo_web_app/commit/86934f2)
* [Dockerize the demo_web_app](https://github.com/learndocker/demo_web_app/commit/0edb9c9)

## Commands
```sh
script/setup-env.sh
docker-compose up -d
docker-compose run app bundle exec rspec
```
