---
lesson_id: 16a77f696556
title: Data in containers
permalink: "/fundamentals/getting-started/data-in-containers/"
course: fundamentals
vimeo: '259597727'
type: video
discussion_id: 16a77f696556
---

## Changes to the examples
* [Add a simple html page](https://github.com/learndocker/docker_examples/commit/f6ea9a4)

## Commands
```sh
docker container run -p 80:80 -v /Users/julian/workspace/docker_examples/html:/usr/share/nginx/html nginx
```

## Sample index.html
```html
<!DOCTYPE html>
<html>
  <body>
    <h1>This is a simple test</h1>
    <p>This is a simple test</p>
  </body>
</html>
```
