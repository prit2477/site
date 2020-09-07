---
lesson_id: 2fed0ac6a5b6
title: Managing configurations
permalink: "/utilizing/running-services/managing-configurations/"
course: utilizing
vimeo: '259617616'
type: assignment
discussion_id: 2fed0ac6a5b6
---

## Preparation for the video
* [Modify the docker-stack.yml to support the assignment](https://github.com/learndocker/docker_examples/commit/193fde9)

## Changes to the examples
* [Add the assignment to use Docker configs](https://github.com/learndocker/docker_examples/commit/5a7ab53)

## Links
* [Configs with Docker Swarm](https://docs.docker.com/engine/swarm/configs/)
* [Configs in the Compose file](https://docs.docker.com/compose/compose-file/#configs)

## The files
* You need to store all the files in a single directory

#### docker-stack.yml
```
version: "3.4"

services:
  frontend:
    image: jfahrer/swarm-demo-frontend:v8
    secrets:
      - pg_secret
    env_file:
      - app.env
    deploy:
      replicas: 10
      update_config:
        failure_action: rollback
        parallelism: 3
        delay: 3s
        max_failure_ratio: 0.1

  db:
    image: jfahrer/swarm-demo-db:v1
    env_file:
      - db.env
    secrets:
      - pg_secret
    volumes:
      - pg-data:/var/lib/postgresql/data
    deploy:
      resources:
        reservations:
          memory: 256M
      placement:
        constraints:
          - node.hostname == node1

  lb:
    image: jfahrer/swarm-demo-lb:v1
    environment:
      - PROXY_UPSTREAM=frontend:8080
    ports:
      - 80:80
    deploy:
      replicas: 3

volumes:
  pg-data:

secrets:
  pg_secret:
    file: ./pg_secret
```

### app.env
```
POSTGRES_USER=demo
POSTGRES_PASSWORD_FILE=/run/secrets/pg_secret
POSTGRES_DB=demo
POSTGRES_HOST=db
```

### db.env
```
POSTGRES_USER=demo
POSTGRES_PASSWORD_FILE=/run/secrets/pg_secret
POSTGRES_DB=demo
```

### pg_secret
```
secret
```
