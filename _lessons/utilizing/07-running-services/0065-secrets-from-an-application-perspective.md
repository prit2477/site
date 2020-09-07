---
lesson_id: 7f3ec75078df
title: Secrets from an application perspective
permalink: "/utilizing/running-services/secrets-from-an-application-perspective/"
course: utilizing
vimeo: '259617554'
type: video
discussion_id: 7f3ec75078df
---

## Changes to the examples
* [Add the files for the secrets example](https://github.com/learndocker/docker_examples/commit/b2af6f8)

## Commands
```sh
echo 'test1234' | docker secret create my-password -
docker stack deploy -c docker-stack.yml test
docker container exec -it test_shell.1.pu3mhzz2tmudecsiziumsfdq sh
cd /run/secrets
ls -l
cat my-password
```
