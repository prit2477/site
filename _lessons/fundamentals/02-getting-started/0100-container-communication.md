---
lesson_id: 64aa65ae8251
title: Container communication
permalink: "/fundamentals/getting-started/container-communication/"
course: fundamentals
vimeo: '259597733'
type: video
discussion_id: 64aa65ae8251
---

## Commands
### First terminal
```sh
docker container run --rm -it --name c1 alpine sh
ping 172.16.0.3
ping c1
cat /etc/hosts
```

### Second terminal
```sh
docker container run --rm -it --name c2 alpine sh
ping 172.16.0.2
docker container run --rm -it --name c2 --link c1 alpine sh
ping c1
```
