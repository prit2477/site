---
title: Docker Fundamentals
weight: 2
image: /uploads/fundamentals.jpg
excerpt: Learn about building and running containers using Docker.

sections:
  - title: Installing Docker
    lessons:
    - "/fundamentals/installing-docker/introduction/"
    - "/fundamentals/installing-docker/what-to-install/"
    - "/fundamentals/installing-docker/docker-for-mac/"
    - "/fundamentals/installing-docker/docker-for-windows/"
    - "/fundamentals/installing-docker/linux/"
    - "/fundamentals/installing-docker/docker-toolbox/"
    - "/fundamentals/installing-docker/docker-machine/"
    - "/fundamentals/installing-docker/creating-docker-machines/"
    - "/fundamentals/installing-docker/creating-docker-machines-ii/"
  - title: Getting started
    lessons:
    - "/fundamentals/getting-started/introduction/"
    - "/fundamentals/getting-started/running-your-first-container/"
    - "/fundamentals/getting-started/starting-a-shell/"
    - "/fundamentals/getting-started/finding-images/"
    - "/fundamentals/getting-started/letting-things-run/"
    - "/fundamentals/getting-started/cleaning-things-up/"
    - "/fundamentals/getting-started/hints/"
    - "/fundamentals/getting-started/publishing-a-service/"
    - "/fundamentals/getting-started/data-in-containers/"
    - "/fundamentals/getting-started/isolation/"
    - "/fundamentals/getting-started/container-communication/"
    - "/fundamentals/getting-started/user-defined-networks/"
    - "/fundamentals/getting-started/the-cli/"
    - "/fundamentals/getting-started/hiding-legacy-commands/"
    - "/fundamentals/getting-started/getting-help/"
  - title: Image basics
    lessons:
    - "/fundamentals/image-basics/introduction/"
    - "/fundamentals/image-basics/what-is-an-image/"
    - "/fundamentals/image-basics/managing-images/"
    - "/fundamentals/image-basics/repositories-and-tags/"
    - "/fundamentals/image-basics/registries/"
    - "/fundamentals/image-basics/creating-a-docker-id/"
    - "/fundamentals/image-basics/meet-docker-hub/"
    - "/fundamentals/image-basics/docker-store/"
    - "/fundamentals/image-basics/docker-login/"
    - "/fundamentals/image-basics/creating-images/"
    - "/fundamentals/image-basics/comments/"
    - "/fundamentals/image-basics/pushing-images/"
    - "/fundamentals/image-basics/docker-cloud/"
    - "/fundamentals/image-basics/hub-store-cloud/"
    - "/fundamentals/image-basics/docker-plugins/"
    - "/fundamentals/image-basics/using-a-3rd-party-registry/"
    - "/fundamentals/image-basics/your-own-image/"
  - title: Container lifecycle
    lessons:
    - "/fundamentals/container-lifecycle/introduction/"
    - "/fundamentals/container-lifecycle/detaching-and-attaching/"
    - "/fundamentals/container-lifecycle/visit-your-container/"
    - "/fundamentals/container-lifecycle/interacting-with-containers/"
    - "/fundamentals/container-lifecycle/stopping-a-container/"
    - "/fundamentals/container-lifecycle/the-end-of-containers/"
    - "/fundamentals/container-lifecycle/debugging-the-issue-from-the-last-assignment/"
    - "/fundamentals/container-lifecycle/becoming-pid1/"
    - "/fundamentals/container-lifecycle/verify-it-is-pid1/"
    - "/fundamentals/container-lifecycle/reading-logs/"
    - "/fundamentals/container-lifecycle/producing-logs/"
    - "/fundamentals/container-lifecycle/using-logfiles/"
    - "/fundamentals/container-lifecycle/logging-errors/"
  - title: Persisting data
    lessons:
    - "/fundamentals/persisting-data/introduction/"
    - "/fundamentals/persisting-data/mounting-data/"
    - "/fundamentals/persisting-data/shortening-the-command/"
    - "/fundamentals/persisting-data/the-mount-option/"
    - "/fundamentals/persisting-data/volumes/"
    - "/fundamentals/persisting-data/naming-volumes/"
    - "/fundamentals/persisting-data/using-mount-for-volumes/"
    - "/fundamentals/persisting-data/managing-volumes/"
    - "/fundamentals/persisting-data/disappearing-volumes/"
    - "/fundamentals/persisting-data/the-volumes-instruction/"
    - "/fundamentals/persisting-data/simultaneous-access/"
    - "/fundamentals/persisting-data/using-volumes-from-other-containers/"
    - "/fundamentals/persisting-data/prepopulating-volumes/"
    - "/fundamentals/persisting-data/when-to-use-volumes/"
  - title: Data in images
    lessons:
    - "/fundamentals/data-in-images/introduction/"
    - "/fundamentals/data-in-images/copying-data/"
    - "/fundamentals/data-in-images/using-wildcards/"
    - "/fundamentals/data-in-images/copying-multiple-files/"
    - "/fundamentals/data-in-images/the-magic-of-add/"
    - "/fundamentals/data-in-images/ignoring-files/"
  - title: Networking 101
    lessons:
    - "/fundamentals/networking-101/introduction/"
    - "/fundamentals/networking-101/publishing-ports/"
    - "/fundamentals/networking-101/publishing-multiple-ports/"
    - "/fundamentals/networking-101/the-expose-instruction/"
    - "/fundamentals/networking-101/what-will-be-published/"
    - "/fundamentals/networking-101/links/"
    - "/fundamentals/networking-101/user-defined-networks/"
    - "/fundamentals/networking-101/resolving-hostnames/"
    - "/fundamentals/networking-101/user-defined-networks-and-links/"
    - "/fundamentals/networking-101/sharing-names/"
  - title: Container behavior
    lessons:
    - "/fundamentals/container-behavior/introduction/"
    - "/fundamentals/container-behavior/the-environment/"
    - "/fundamentals/container-behavior/the-env-instruction/"
    - "/fundamentals/container-behavior/more-on-env-vars/"
    - "/fundamentals/container-behavior/postgres-in-a-nutshell/"
    - "/fundamentals/container-behavior/configuring-postgres/"
    - "/fundamentals/container-behavior/using-the-database/"
    - "/fundamentals/container-behavior/try-it-out/"
    - "/fundamentals/container-behavior/multiple-containers/"
    - "/fundamentals/container-behavior/how-it-works/"
  - title: Scaling a web service
    lessons:
    - "/fundamentals/scaling-a-web-service/introduction/"
    - "/fundamentals/scaling-a-web-service/what-we-will-build/"
    - "/fundamentals/scaling-a-web-service/a-basic-image/"
    - "/fundamentals/scaling-a-web-service/testing-the-image/"
    - "/fundamentals/scaling-a-web-service/substituting-env-vars/"
    - "/fundamentals/scaling-a-web-service/making-it-dynamic/"
    - "/fundamentals/scaling-a-web-service/running-the-load-balancer/"
    - "/fundamentals/scaling-a-web-service/it-does-not-stop/"
    - "/fundamentals/scaling-a-web-service/using-the-load-balancer/"
    - "/fundamentals/scaling-a-web-service/scaling-the-app/"
  - title: Managing containers with Docker Compose
    lessons:
    - "/fundamentals/managing-containers-with-docker-compose/introduction/"
    - "/fundamentals/managing-containers-with-docker-compose/compose-example/"
    - "/fundamentals/managing-containers-with-docker-compose/an-introduction-to-yaml/"
    - "/fundamentals/managing-containers-with-docker-compose/our-first-compose-file/"
    - "/fundamentals/managing-containers-with-docker-compose/compose-resources/"
    - "/fundamentals/managing-containers-with-docker-compose/configuring-our-database/"
    - "/fundamentals/managing-containers-with-docker-compose/using-a-volume/"
    - "/fundamentals/managing-containers-with-docker-compose/interacting-with-containers/"
    - "/fundamentals/managing-containers-with-docker-compose/integrate-the-demo_web_app/"
    - "/fundamentals/managing-containers-with-docker-compose/managing-environment-variables/"
    - "/fundamentals/managing-containers-with-docker-compose/specifying-dependencies/"
    - "/fundamentals/managing-containers-with-docker-compose/limitations-of-depends_on/"
    - "/fundamentals/managing-containers-with-docker-compose/integrate-the-load-balancer/"
    - "/fundamentals/managing-containers-with-docker-compose/enhancing-the-load-balancer/"
    - "/fundamentals/managing-containers-with-docker-compose/building-the-load-balancer/"
    - "/fundamentals/managing-containers-with-docker-compose/scaling-a-service/"

---

The Docker Fundamentals course will get you up to speed with building and running containers using Docker. We will teach you the core concepts around Docker and containers. You will become familiar with the tooling around Docker and learn how to apply best practices. We will take you all the way from installing Docker on your machine to spinning up multiple containers that communicate with each other.

This course teaches the fundamental knowledge required in the other courses. If you’re already familiar with Docker, I generally recommend watching the videos at a higher speed rather than skipping them.