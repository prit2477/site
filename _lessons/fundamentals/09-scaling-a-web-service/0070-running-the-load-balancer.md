---
lesson_id: 76117bfbce4e
title: Running the load balancer
permalink: "/fundamentals/scaling-a-web-service/running-the-load-balancer/"
course: fundamentals
vimeo: '259609888'
type: video
discussion_id: 76117bfbce4e
---

## Changes to the examples
* [Make the start.sh executable](https://github.com/learndocker/docker_examples/commit/83f96c2)

## Commands
```sh
chmod +x script.sh
docker image build -t jfahrer/lb:latest .
docker container run --network mynet -p 80:80 jfahrer/lb:latest
```
