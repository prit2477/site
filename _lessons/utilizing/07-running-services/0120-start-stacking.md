---
lesson_id: 975fd0dbe9a1
title: Start stacking
permalink: "/utilizing/running-services/start-stacking/"
course: utilizing
vimeo: '259617788'
type: assignment
discussion_id: 975fd0dbe9a1
---

## Changes to the examples
* [Add the assignment to play around with stacks](https://github.com/learndocker/docker_examples/commit/3dc2be8)

## Links
* [Placement preferences](https://docs.docker.com/engine/reference/commandline/service_create/#specify-service-placement-preferences-placement-pref)
* [Placement of services](https://docs.docker.com/compose/compose-file/#placement)
* [Resources in a Compose file](https://docs.docker.com/compose/compose-file/#resources)

## Images
* [jfahrer/swarm-demo-frontend](https://store.docker.com/community/images/jfahrer/swarm-demo-frontend)
* [jfahrer/swarm-demo-db](https://store.docker.com/community/images/jfahrer/swarm-demo-db)
* [jfahrer/swarm-demo-lb](https://store.docker.com/community/images/jfahrer/swarm-demo-lb)

## The tags
* `v1` [(swarm-demo-frontend/v1/Dockerfile)](https://github.com/learndocker/example_images/blob/master/swarm-demo-frontend/v1/Dockerfile)

  The initial version. This version has no external dependencies and runs a web server on port 8080 

* `v2`  [(swarm-demo-frontend/v2/Dockerfile)](https://github.com/learndocker/example_images/blob/master/swarm-demo-frontend/v2/Dockerfile)

  Like `v1` but with a grey background

* `v3`:  [(swarm-demo-frontend/v3/Dockerfile)](https://github.com/learndocker/example_images/blob/master/swarm-demo-frontend/v3/Dockerfile)

  This version is manipulated and the main process will die on startup

* `v4`  [(swarm-demo-frontend/v4/Dockerfile)](https://github.com/learndocker/example_images/blob/master/swarm-demo-frontend/v4/Dockerfile)

  This version fixes the issue of `v3` and set the background color to white.

* `v5`:  [(swarm-demo-frontend/v5/Dockerfile)](https://github.com/learndocker/example_images/blob/master/swarm-demo-frontend/v5/Dockerfile)

   This version introduces PostgreSQL as an external dependency. Requests are logged and stored in a database. The last 25 requests will be read from the database and listed.

* `v6` [(swarm-demo-frontend/v6/Dockerfile)](https://github.com/learndocker/example_images/blob/master/swarm-demo-frontend/v6/Dockerfile)

  Like `v5` but 30 instead of 25 will be read from the database and listed.

* `v7` [(swarm-demo-frontend/v7/Dockerfile)](https://github.com/learndocker/example_images/blob/master/swarm-demo-frontend/v7/Dockerfile)

  This version will fail on startup. It can be used to test failing updates.

* `v8`:  [(swarm-demo-frontend/v8/Dockerfile)](https://github.com/learndocker/example_images/blob/master/swarm-demo-frontend/v8/Dockerfile)

  Introduced support for using Docker Secrets to set the PostgreSQL password. 

* `v9`  [(swarm-demo-frontend/v9/Dockerfile)](https://github.com/learndocker/example_images/blob/master/swarm-demo-frontend/v9/Dockerfile)

  Adds the ability to define the number of requests to display via an environment variable. This tag can be used to test updates.

* `v10`  [(swarm-demo-frontend/v10/Dockerfile)](https://github.com/learndocker/example_images/blob/master/swarm-demo-frontend/v10/Dockerfile)

  Add a `/status` endpoint to support health checks. Health checks using this endpoint will randomly fail after a certain amount of checks. This version can be used to test auto-healing capabilities of Docker Swarm.

* `v11`  [(swarm-demo-frontend/v11/Dockerfile)](https://github.com/learndocker/example_images/blob/master/swarm-demo-frontend/v11/Dockerfile)

  The`/status` endpoint of this version is fixed and works as expected. Health checks will not randomly fail.

## Configuration
The application supports the following environment variables:
* `POSTGRES_HOST` (`v5` and higher): The hostname of the machine or container that runs the PostgreSQL database. The app will try to connect to this host.  
* `POSTGRES_DB` (`v5` and higher): The database name that will be used. Make sure that the database exists.
* `POSTGRES_USER` (`v5` and higher):  The username that will be used to connect to the PostgreSQL database.
* `POSTGRES_PASSWORD` (`v5` and higher):  The password that is used to connect to the PostgreSQL database. The default is no password.
* `POSTGRES_PASSWORD_FILE` (`v8` and higher): The path to the file containing the password to connect to the PostgreSQL database. This can be used in combination with Docker Secrets.
* `NUMBER_OF_REQUESTS` (`v9` and higher): Controls the number of requests that will be shown on the homepage.
* `MIN_REQUESTS_TILL_DEATH` (`v10` only): The minimum number of health checks that will succeed.
* `MAX_REQUESTS_TILL_DEATH` (`v10` only): The maximum number of health checks that will succeed.

Please make sure to set the `POSTGRES_PASSWORD` environment variable if you are using a version < `v8`.

## The files
* All the files can be found in this [GitHub repository](https://github.com/learndocker/stack_example)
* You can also download an archive with all files from [here](https://github.com/learndocker/stack_example/archive/master.zip)
