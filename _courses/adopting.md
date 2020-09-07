---
title: Adopting Docker
weight: 4
image: /uploads/adopting.jpg
excerpt: Adopting Docker for your existing applications and integrating it into your infrastructure.

sections:
  - title: Introduction
    lessons:
    - "/adopting/introduction/what-to-expect/"
    - "/adopting/introduction/cncf/"
  - title: Swarm in production
    lessons:
    - "/adopting/swarm-in-production/installing-nodes/"
    - "/adopting/swarm-in-production/cluster-setup/"
    - "/adopting/swarm-in-production/draining-nodes-and-rebalancing-tasks/"
    - "/adopting/swarm-in-production/operating-a-cluster/"
    - "/adopting/swarm-in-production/losing-quorum/"
    - "/adopting/swarm-in-production/labels/"
    - "/adopting/swarm-in-production/cross-stack-communication/"
  - title: Dealing with dependencies
    lessons:
    - "/adopting/dealing-with-dependencies/introduction/"
    - "/adopting/dealing-with-dependencies/bootstrapping-a-project/"
    - "/adopting/dealing-with-dependencies/installing-dependencies/"
    - "/adopting/dealing-with-dependencies/extracting-data-from-containers/"
    - "/adopting/dealing-with-dependencies/bind-mounts-and-the-workdir/"
    - "/adopting/dealing-with-dependencies/utilizing-the-build-cache/"
    - "/adopting/dealing-with-dependencies/system-libraries-and-utilities/"
    - "/adopting/dealing-with-dependencies/waiting-for-external-dependencies/"
  - title: Developing with Docker
    lessons:
    - "/adopting/developing-with-docker/introduction/"
    - "/adopting/developing-with-docker/non-persistent-application-state/"
    - "/adopting/developing-with-docker/monoliths-vs-microservices/"
    - "/adopting/developing-with-docker/keeping-build-time-secrets-a-secret/"
    - "/adopting/developing-with-docker/testing-applications/"
    - "/adopting/developing-with-docker/preparing-the-environment/"
    - "/adopting/developing-with-docker/seperating-environments/"
    - "/adopting/developing-with-docker/application-specific-environments/"
    - "/adopting/developing-with-docker/dockerizing-applications/"
    - "/adopting/developing-with-docker/docker-and-12-factor-apps/"
  - title: Continous Integration
    lessons:
    - "/adopting/continous-integration/what-we-will-do/"
    - "/adopting/continous-integration/the-application/"
    - "/adopting/continous-integration/integrating-circleci/"
    - "/adopting/continous-integration/running-the-test-suite/"
    - "/adopting/continous-integration/extracting-artifacts/"
    - "/adopting/continous-integration/building-images/"
    - "/adopting/continous-integration/docker-cloud/"
    - "/adopting/continous-integration/deploying-applications/"
    - "/adopting/continous-integration/build-your-own-images/"
    - "/adopting/continous-integration/restoring-the-build-cache/"
  - title: Logging
    lessons:
    - "/adopting/logging/what-we-will-do/"
    - "/adopting/logging/integrating-fluentd/"
    - "/adopting/logging/forwarding-logs/"
    - "/adopting/logging/integrating-loggly/"
    - "/adopting/logging/tagging-logs/"
    - "/adopting/logging/the-json-file-driver/"
    - "/adopting/logging/the-default-logging-driver/"
    - "/adopting/logging/docker-events/"
    - "/adopting/logging/daemon-logs/"
  - title: Learning more
    lessons:
    - "/adopting/learning-more/cncf-landscape/"
    - "/adopting/learning-more/kubernetes/"
    - "/adopting/learning-more/keeping-up/"


---

We are going to focus on understanding the moving parts and choices you can make in adopting Docker for your existing applications and integrating it into your infrastructure. This way you can come up with solutions that meet your requirements for your projects.

Additionally, we will look into how to set up a production infrastructure and tackle things like logging and monitoring. We will also go over some of the caveats you might encounter when Dockerizing your applications.