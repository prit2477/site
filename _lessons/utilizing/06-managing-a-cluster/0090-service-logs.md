---
lesson_id: b5699ff0390e
title: Service logs
permalink: "/utilizing/managing-a-cluster/service-logs/"
course: utilizing
vimeo: '259616461'
type: video
discussion_id: b5699ff0390e
---

## Commands
```sh
docker service ls
docker service update --image jfahrer/swarm-demo-frontend:v3 --update-failure-action rollback --update-parallelism 3 demo-frontend
docker service logs ovmxnalrncrh
docker service logs --help
```
