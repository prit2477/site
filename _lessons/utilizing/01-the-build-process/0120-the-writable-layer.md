---
lesson_id: c06542fd3fa6
title: The writable layer
permalink: "/utilizing/the-build-process/the-writable-layer/"
course: utilizing
vimeo: '259610185'
type: video
discussion_id: c06542fd3fa6
---

## Links
* [Container size on disk](https://docs.docker.com/storage/storagedriver/#container-size-on-disk)

## Commands
```sh
docker container run -itd alpine:latest sh
docker container ls -s
docker image ls alpine:latest
docker container run -d alpine:latest dd if=/dev/random of=/test.file
docker container ls -s
```
