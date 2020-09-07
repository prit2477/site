---
lesson_id: 3fbb9ca4ee6d
title: Adding a database
permalink: "/utilizing/writing-code/adding-a-database/"
course: utilizing
vimeo: '259610293'
type: video
discussion_id: 3fbb9ca4ee6d
---

## Changes to the examples
* [Add the pg service to the compose file](https://github.com/learndocker/docker_examples/commit/e6138f0)
* [Add the file with the SQL statement to create the table](https://github.com/learndocker/docker_examples/commit/d096d23)
* [Add the bind mount for the pg service](https://github.com/learndocker/docker_examples/commit/13d3f1a)

## Links
* [The postgres image](https://store.docker.com/images/postgres)

## The SQL statement
```
CREATE TABLE IF NOT EXISTS requests (
  id serial primary key,
  requested_at character varying,
  ip character varying,
  host character varying,
  path character varying
);
```
