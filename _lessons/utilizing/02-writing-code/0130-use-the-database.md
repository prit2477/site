---
lesson_id: f34238344b71
title: Use the database
permalink: "/utilizing/writing-code/use-the-database/"
course: utilizing
vimeo: '259610299'
type: assignment
discussion_id: f34238344b71
---

## Changes to the examples
* [Add the third assignment to use the database](https://github.com/learndocker/docker_examples/commit/003f3c9)
* [Install the system and language libraries](https://github.com/learndocker/docker_examples/commit/791c6a3)
* [Connect to the database postgres and store requests inside the database](https://github.com/learndocker/docker_examples/commit/8b67cda)
* [Integrate the client file into the compoe file](https://github.com/learndocker/docker_examples/commit/732d0f9)
* [Implement the third assignment in ruby](https://github.com/learndocker/docker_examples/commit/f23c7ac)

## Links
* [The client](https://store.docker.com/community/images/jfahrer/checker-u-dev-a3)

## The SQL statment
```
INSERT INTO requests (ip, path, host, requested_at)
VALUES ('127.21.0.4', '/', '8e358f1ba0db', '2018-01-09 10:38:10 +0000');
```
