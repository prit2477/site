---
lesson_id: 5de32a12ee6c
title: Creating nodes with docker-machine
permalink: "/utilizing/managing-a-cluster/creating-nodes-with-docker-machine/"
course: utilizing
vimeo: '259616200'
type: video
discussion_id: 5de32a12ee6c
---

## Links
* [Machine drivers](https://docs.docker.com/machine/drivers/)
* [Digital Ocean ($10 referral code)](https://m.do.co/c/58b72192f338)
* [How To Set Up SSH Keys](https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys--2)

## Commands
```sh
docker-machien create --driver vmwarefusion --vmwarefusion-cpu-count 1 --vmwarefusion-memory-size 1024 node1
docker-machien create --driver vmwarefusion --vmwarefusion-cpu-count 1 --vmwarefusion-memory-size 1024 node2
docker-machien create --driver vmwarefusion --vmwarefusion-cpu-count 1 --vmwarefusion-memory-size 1024 node3
docker-machine ls
docker-machine env node1
docker-machine ssh node2
docker-machine create --driver generic --generic-ip-address=1.1.1.1 --generic-ssh-key ~/.ssh/id_rsa do-node1
```
