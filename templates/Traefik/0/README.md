# Traefik
### Version: 1.6 ≤ x ≤ 1.7

Traefik is a modern HTTP reverse proxy and load balancer that makes deploying microservices easy. Traefik integrates with your existing infrastructure components (Docker, Swarm mode, Kubernetes, Marathon, Consul, Etcd, Rancher, Amazon ECS, ...) and configures itself automatically and dynamically. Pointing Traefik at your orchestrator should be the only configuration step you need.

## About

## Pre-Depoloyment

* Create a "traefik.toml" file to configure Traefik how you would like for it to function
  * This will go in the `<Stack Directory>/Configuration` directory
  * Examples for what it should contain:
    * [Docker](https://docs.traefik.io/configuration/backends/docker/)
    * [Rancher](https://docs.traefik.io/configuration/backends/rancher/)
