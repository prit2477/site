---
lesson_id: a618b4f5b6fd
title: Using the load balancer
permalink: "/fundamentals/scaling-a-web-service/using-the-load-balancer/"
course: fundamentals
vimeo: '259609909'
type: assignment
discussion_id: a618b4f5b6fd
---

## Changes to the examples
* [Add the assignment](https://github.com/learndocker/docker_examples/commit/bfd3e2d)

## Images
* [postgres](https://store.docker.com/images/postgres)
* [jfahrer/demo_web_app](https://store.docker.com/community/images/jfahrer/demo_web_app)

## The Dockerfile
```Dockerfile
FROM jfahrer/nginx:latest

RUN apt-get update && apt-get install gettext-base

ENV PROXY_PROTOCOL=http PROXY_UPSTREAM=example.com

COPY proxy.conf /etc/nginx/sites-available/default.template
COPY start.sh /

CMD ["/start.sh"]
```


## The start.sh script
```sh
#!/usr/bin/env bash

envsubst '$PROXY_PROTOCOL,$PROXY_UPSTREAM' < /etc/nginx/sites-available/default.template > /etc/nginx/sites-available/default
exec nginx -g 'daemon off;'
```

## The proxy.conf
```conf
server {
  listen 80 default_server;

  resolver 127.0.0.11;

  set $protocol $PROXY_PROTOCOL;
  set $upstream $PROXY_UPSTREAM;

  location / {
    proxy_pass $protocol://$upstream$request_uri;

    proxy_pass_header Authorization;

    proxy_http_version 1.1;
    proxy_ssl_server_name on;
    proxy_set_header Host $upstream;
    proxy_set_header X-Real-IP $remote_addr;
    proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
    proxy_set_header Connection "";

    proxy_buffering off;
    proxy_read_timeout 5s;
    proxy_redirect off;
    proxy_ssl_verify off;
    client_max_body_size 0;
  }
}
```
