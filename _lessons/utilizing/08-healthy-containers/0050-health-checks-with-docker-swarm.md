---
lesson_id: 3cca48531ed9
title: Health Checks with Docker Swarm
permalink: "/utilizing/healthy-containers/health-checks-with-docker-swarm/"
course: utilizing
vimeo: '259617879'
type: video
discussion_id: 3cca48531ed9
---

## Commands
```sh
docker-compose -f docker-compose.yml -f docker-compose.prod.yml config > docker-stack.yml
docker stack deploy -c docker-stack.yml demo
watch docker stack services demo
```
