---
lesson_id: c7c559a75b15
title: Build arguments and secrets
permalink: "/utilizing/optimal-images/build-arguments-and-secrets/"
course: utilizing
vimeo: '259610489'
type: video
discussion_id: c7c559a75b15
---

## Commands
```sh
docker image build -t secrets --build-arg PASSWORD=test .
docker image history secrets
```
