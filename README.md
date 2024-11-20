# Home Lab Services

This repository contains a collection of services that I run in my home lab. The services are managed using Docker and Docker Compose.

## Pi-hole

Pi-hole is a network-wide ad blocker. It blocks ads on all devices connected to the network.

### Usage

```bash
$ docker compose --env-file .env --file pihole/docker-compose.yml up -d
```

## Prometheus

Prometheus is a monitoring and alerting toolkit.

The following services are included in the Prometheus stack:

- Prometheus
- Node Exporter (for monitoring the host machine)

### Usage

```bash
$ docker compose --env-file .env --file prometheus/docker-compose.yml up -d
```
