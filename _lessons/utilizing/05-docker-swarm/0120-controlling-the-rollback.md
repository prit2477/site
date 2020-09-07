---
lesson_id: 2b6c2c9d2a96
title: Controlling the Rollback
permalink: "/utilizing/docker-swarm/controlling-the-rollback/"
course: utilizing
vimeo: '259610714'
type: video
discussion_id: 2b6c2c9d2a96
---

## Commands
```sh
docker service update --rollback --help | grep rollback
docker service update --update-failure-action rollback --update-parallelism 3 --update-monitor 10s --image jfahrer/swarm-demo-frontend:v3 --rollback-parallelism 3 publish-demo
```
