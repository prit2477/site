---
lesson_id: b7400db79a80
title: List requests
permalink: "/utilizing/writing-code/list-requests/"
course: utilizing
vimeo: '259610305'
type: assignment
discussion_id: b7400db79a80
---

## Changes to the examples
* [Add the fourth assignment](https://github.com/learndocker/docker_examples/commit/b2acfa2)
* [Display a list of requests retrieved from the database](https://github.com/learndocker/docker_examples/commit/6119d58)
* [Implement the fourth assignment in ruby](https://github.com/learndocker/docker_examples/commit/123c3e7)

## The SQL statement
```
SELECT ip, path, host, requested_at
FROM requests
ORDER BY id DESC
LIMIT 25;
```
