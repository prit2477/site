---
lesson_id: 3da88e2e8bc1
title: Testing the image
permalink: "/fundamentals/scaling-a-web-service/testing-the-image/"
course: fundamentals
vimeo: '259609868'
type: video
discussion_id: 3da88e2e8bc1
---

## Commands
```sh
docker image build -t jfahrer/lb:latest .
docker network create mynet
docker container run --network mynet -p 80:80 jfahrer/lb:latest
```
