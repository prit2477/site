---
lesson_id: 8fa13f8ff4bc
title: Use an ENTRYPOINT
permalink: "/utilizing/running-containers/use-an-entrypoint/"
course: utilizing
vimeo: '259610415'
type: video
discussion_id: 8fa13f8ff4bc
---

## Changes to the examples
* [Change the load balancer to use official nginx image](https://github.com/learndocker/docker_examples/commit/d26c414)
* [Add the assignment to use and ENTRYPOINT](https://github.com/learndocker/docker_examples/commit/82b5be7)

## Links
* [ENTRYPOINT](https://docs.docker.com/engine/reference/builder/#entrypoint)

## The files
### Dockerfile
```
FROM nginx:1.13.8

ENV PROXY_PROTOCOL=http PROXY_UPSTREAM=example.com

COPY proxy.conf /etc/nginx/conf.d/default.template
COPY start.sh /

CMD ["/start.sh"]
```

### start.sh
```
#!/usr/bin/env bash
envsubst '$PROXY_PROTOCOL,$PROXY_UPSTREAM' < /etc/nginx/conf.d/default.template > /etc/nginx/conf.d/default.conf

exec nginx -g 'daemon off;'
```

### proxy.conf
```
server {
  listen 80 default_server;

  resolver 127.0.0.11 valid=1s;

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
