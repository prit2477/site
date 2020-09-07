---
lesson_id: ff637471825e
title: User defined networks
permalink: "/fundamentals/getting-started/user-defined-networks/"
course: fundamentals
vimeo: '259597737'
type: video
discussion_id: ff637471825e
---

## Commands
```sh
docker network ls
docker network create test
docker container run -it --rm --network test --name c1 alpine sh
```

In a second terminal:
```sh
docker container run -it --rm --network test --name c2 alpine sh
ping c1
```

To clean up:
```sh
docker network rm test
```
