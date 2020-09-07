---
lesson_id: cfaf06de6fea
title: Draining nodes and rebalancing tasks
permalink: "/adopting/swarm-in-production/draining-nodes-and-rebalancing-tasks/"
course: adopting
vimeo: '259618037'
type: video
discussion_id: cfaf06de6fea
---

## Commands
```sh
docker node ls
docker service ls
docker service ps --filter node=node2 demo_frontend
docker node update availability=drain node2
docker node ls
docker node update availability=active node2
docker update -f demo_frontend
docker service scale demo_frontend=13
docker service scale demo_frontend=10
```
