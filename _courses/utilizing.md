---
title: Utilizing Docker
weight: 3
image: /uploads/utilizing.jpg
excerpt: Once you have mastered the Docker fundamentals, it is time to dig deeper. 

sections:
  - title: The build process
    lessons:
    - "/utilizing/the-build-process/a-side-note/"
    - "/utilizing/the-build-process/understanding-layers/"
    - "/utilizing/the-build-process/creating-layers/"
    - "/utilizing/the-build-process/the-build-process/"
    - "/utilizing/the-build-process/how-the-cache-works/"
    - "/utilizing/the-build-process/invalidating-the-cache/"
    - "/utilizing/the-build-process/copy-and-add/"
    - "/utilizing/the-build-process/dangling-images/"
    - "/utilizing/the-build-process/leightweight-images/"
    - "/utilizing/the-build-process/using-multiple-lines/"
    - "/utilizing/the-build-process/optimize-the-nginx-image/"
    - "/utilizing/the-build-process/the-writable-layer/"
  - title: Writing code
    lessons:
    - "/utilizing/writing-code/introduction/"
    - "/utilizing/writing-code/hello-world/"
    - "/utilizing/writing-code/compiled-languages/"
    - "/utilizing/writing-code/the-dockerfiles/"
    - "/utilizing/writing-code/picking-an-image/"
    - "/utilizing/writing-code/your-turn/"
    - "/utilizing/writing-code/iterating-with-docker-and-compose/"
    - "/utilizing/writing-code/running-commands/"
    - "/utilizing/writing-code/starting-a-web-server/"
    - "/utilizing/writing-code/the-implementation/"
    - "/utilizing/writing-code/interlude/"
    - "/utilizing/writing-code/storing-requests/"
    - "/utilizing/writing-code/adding-a-database/"
    - "/utilizing/writing-code/use-the-database/"
    - "/utilizing/writing-code/list-requests/"
    - "/utilizing/writing-code/integrate-your-load-balancer/"
  - title: Running containers
    lessons:
    - "/utilizing/running-containers/introduction/"
    - "/utilizing/running-containers/container-statistics/"
    - "/utilizing/running-containers/limiting-resources/"
    - "/utilizing/running-containers/docker-compose-and-resources/"
    - "/utilizing/running-containers/using-a-tmpfs/"
    - "/utilizing/running-containers/running-nginx-read-only/"
    - "/utilizing/running-containers/changing-the-user/"
    - "/utilizing/running-containers/docker-security/"
    - "/utilizing/running-containers/entrypoints/"
    - "/utilizing/running-containers/entrypoints-and-custom-commands/"
    - "/utilizing/running-containers/command-line-containers/"
    - "/utilizing/running-containers/use-an-entrypoint/"
    - "/utilizing/running-containers/one-concern-per-container/"
  - title: Optimal images
    lessons:
    - "/utilizing/optimal-images/build-arguments/"
    - "/utilizing/optimal-images/build-arguments-in-compose/"
    - "/utilizing/optimal-images/dynamic-cmd-instructions/"
    - "/utilizing/optimal-images/environment-replacement/"
    - "/utilizing/optimal-images/add-a-build-argument-to-nginx/"
    - "/utilizing/optimal-images/docker-compose-and-environment-variables/"
    - "/utilizing/optimal-images/build-arguments-and-secrets/"
    - "/utilizing/optimal-images/onbuild/"
    - "/utilizing/optimal-images/updating-base-images/"
    - "/utilizing/optimal-images/pinning-images/"
    - "/utilizing/optimal-images/utilizing-the-build-cache/"
    - "/utilizing/optimal-images/multistage-builds/"
    - "/utilizing/optimal-images/documentation/"
    - "/utilizing/optimal-images/stopping-gracefully/"
    - "/utilizing/optimal-images/properly-tagging-images/"
  - title: Docker Swarm
    lessons:
    - "/utilizing/docker-swarm/meet-docker-swarm/"
    - "/utilizing/docker-swarm/swarm-vs-kubernetes/"
    - "/utilizing/docker-swarm/single-node-swarm/"
    - "/utilizing/docker-swarm/creating-a-service/"
    - "/utilizing/docker-swarm/tasks-and-containers/"
    - "/utilizing/docker-swarm/deleting-a-service/"
    - "/utilizing/docker-swarm/the-desired-state/"
    - "/utilizing/docker-swarm/publishing-a-service/"
    - "/utilizing/docker-swarm/updating-a-service/"
    - "/utilizing/docker-swarm/controlling-the-update/"
    - "/utilizing/docker-swarm/rolling-back/"
    - "/utilizing/docker-swarm/controlling-the-rollback/"
    - "/utilizing/docker-swarm/the-update-process/"
    - "/utilizing/docker-swarm/interservice-communication/"
    - "/utilizing/docker-swarm/deploy-some-services/"
  - title: Managing a cluster
    lessons:
    - "/utilizing/managing-a-cluster/nodes-managers-and-workers/"
    - "/utilizing/managing-a-cluster/preparing-the-nodes/"
    - "/utilizing/managing-a-cluster/creating-nodes-with-docker-machine/"
    - "/utilizing/managing-a-cluster/creating-the-cluster/"
    - "/utilizing/managing-a-cluster/leaving-the-swarm/"
    - "/utilizing/managing-a-cluster/distributed-services/"
    - "/utilizing/managing-a-cluster/publishing-services-with-multiple-nodes/"
    - "/utilizing/managing-a-cluster/docker-swarm-networking/"
    - "/utilizing/managing-a-cluster/service-logs/"
    - "/utilizing/managing-a-cluster/events/"
    - "/utilizing/managing-a-cluster/dealing-with-volumes/"
    - "/utilizing/managing-a-cluster/volume-plugins/"
    - "/utilizing/managing-a-cluster/service-constraints/"
    - "/utilizing/managing-a-cluster/limiting-resources/"
    - "/utilizing/managing-a-cluster/setting-up-a-demo/"
    - "/utilizing/managing-a-cluster/the-solution/"
  - title: Running services
    lessons:
    - "/utilizing/running-services/stacks/"
    - "/utilizing/running-services/the-stack-file/"
    - "/utilizing/running-services/updating-services-in-a-stack/"
    - "/utilizing/running-services/graceful-updates/"
    - "/utilizing/running-services/managing-secrets/"
    - "/utilizing/running-services/secrets-with-docker-stack/"
    - "/utilizing/running-services/secrets-from-an-application-perspective/"
    - "/utilizing/running-services/managing-configurations/"
    - "/utilizing/running-services/structuring-compose-files-i/"
    - "/utilizing/running-services/structuring-compose-files-ii/"
    - "/utilizing/running-services/structuring-compose-files-iii/"
    - "/utilizing/running-services/docker-stack-and-multiple-compose-files/"
    - "/utilizing/running-services/replication-mode/"
    - "/utilizing/running-services/start-stacking/"
  - title: Healthy containers
    lessons:
    - "/utilizing/healthy-containers/resilient-applications/"
    - "/utilizing/healthy-containers/health-checks/"
    - "/utilizing/healthy-containers/implementing-a-health-check/"
    - "/utilizing/healthy-containers/inspecting-faulty-containers/"
    - "/utilizing/healthy-containers/health-checks-with-docker-swarm/"
    - "/utilizing/healthy-containers/inspecting-faulty-tasks/"
    - "/utilizing/healthy-containers/designing-health-checks/"
    - "/utilizing/healthy-containers/restart-policies/"
    - "/utilizing/healthy-containers/a-restart-policy-in-action/"
    - "/utilizing/healthy-containers/implement-a-health-check/"


---

Once you have mastered the Docker fundamentals, it is time to dig deeper. We will dive into the various aspects of developing and running applications using Docker containers. The goal is to get you to a level where running applications using Docker feels natural to you.

We will be developing applications in various languages and put them into containers. You will get the chance to develop in the language of your choice!

Additionally, you will also learn to use Docker Swarm for container orchestration which will teach you how to deal with a containerized environment in production.