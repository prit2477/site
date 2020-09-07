---
lesson_id: 87bb2d192c1b
title: Creating the cluster
permalink: "/utilizing/managing-a-cluster/creating-the-cluster/"
course: utilizing
vimeo: '259616211'
type: video
discussion_id: 87bb2d192c1b
---

## Commands
```sh
docker swarm init
docker swarm join --token XXX 1.1.1.1:2377
docker node promote node2
docker swarm join-token manager
```
