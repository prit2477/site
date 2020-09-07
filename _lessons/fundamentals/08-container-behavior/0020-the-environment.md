---
lesson_id: c22fabc8f047
title: The environment
permalink: "/fundamentals/container-behavior/the-environment/"
course: fundamentals
vimeo: '259597889'
type: video
discussion_id: c22fabc8f047
---

## Commands
```sh
docker container run jfahrer/myalpine:latest
export PS1='test '
export PS1="\h:\w# "
exit
docker container run -it -e "PS1=\h:\w# " jfahrer/myalpine:latest
```
