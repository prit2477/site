---
lesson_id: 5403b637399a
title: Utilizing the build cache
permalink: "/utilizing/optimal-images/utilizing-the-build-cache/"
course: utilizing
vimeo: '268195062'
type: video
discussion_id: 5403b637399a
---

## Commands
```sh
docker image ls -a
docker image build -t jfahrer/myalpine:bash --cache-from jfahrer/myalpine:bash .
docker image ls -a
docker-compose build
```
