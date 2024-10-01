# docker-homelab

This repository contains Docker Compose configurations for various services used in my homelab. Each service is containerized for easy deployment and management. Below you'll find details for each service, its purpose, and setup instructions.

## Table of Contents

- [AdGuardHome](#adguardhome)
- [Dashy](#dashy)
- [Emby](#emby)
- [Monitoring](#monitoring)
- [Pi-hole](#pi-hole)
- [Portainer](#portainer)
- [qBittorrent](#qbittorrent)

---

## AdGuardHome

### Overview
AdGuardHome is a network-wide ad-blocking DNS server that helps protect your devices from ads, trackers, and other unwanted content.

### Docker Compose Configuration
- File: `docker/adguardhome/docker-compose.yml`
- Description: This Compose file sets up AdGuardHome as a DNS server on the local network. It provides configuration for the service, network settings, and volume mounts.

### Key Features
- Network-wide ad-blocking
- Customizable DNS filtering rules

### Usage
To start the AdGuardHome service, navigate to its directory and run:
```
docker-compose up -d
```


## Dashy

### Overview
Dashy is a beautiful, customizable dashboard for managing all your homelab services and bookmarks in one place.

### Docker Compose Configuration
- File: `docker/dashy/docker-compose.yml`
- Description: This Compose file sets up Dashy with access to its configuration and data directories.

### Key Features
- Easy-to-use dashboard for quick access to services
- Fully customizable with various themes and widgets

### Usage
To start the Dashy service, navigate to its directory and run:
```
docker-compose up -d
```

## Emby

### Overview
Emby is a media server that helps organize and stream your video, audio, and other content to various devices.
Docker Compose Configuration

- File: `docker/emby/docker-compose.yml`
- Description: The Compose file sets up Emby for streaming media from a local directory.

### Key Features
- Media streaming to multiple devices
- Rich metadata fetching for your library

### Usage
To start the Emby service, navigate to its directory and run:
```
docker-compose up -d
```

## Monitoring

### Overview
The monitoring stack includes tools like Prometheus, Grafana, and Node Exporter to help track the performance and health of your homelab infrastructure.

### Docker Compose Configuration
- File: `docker/monitoring/docker-compose.yml`
- Description: This Compose file sets up Prometheus for data collection, Grafana for visualizations, and other monitoring components.

### Key Features
- Metrics collection using Prometheus
- Dashboard visualization with Grafana
- cAdvisor analyzes and exposes resource usage and performance data from running docker containers

### Usage
To start the monitoring stack, navigate to its directory and run:
```
docker-compose up -d
```

## Pi-hole

### Overview
Pi-hole is a DNS-level ad blocker that works as an alternative to AdGuardHome for blocking ads and trackers.

### Docker Compose Configuration
- File: `docker/pihole/docker-compose.yaml`
- Description: This Compose file sets up Pi-hole for managing DNS queries and blocking unwanted domains.

### Key Features
- DNS-level ad blocking
- Web interface for easy configuration

### Usage
To start the Pi-hole service, navigate to its directory and run:
```
docker-compose up -d
```

## Portainer

### Overview
Portainer is a lightweight management UI for Docker, allowing you to easily manage containers, images, volumes, and networks through a web interface.

### Docker Compose Configuration
- File: `docker/portainer/docker-compose.yml`
- Description: This Compose file sets up Portainer with access to Docker's API.

### Key Features
- Web-based Docker management
- Easy deployment of containers

### Usage
To start Portainer, navigate to its directory and run:
```
docker-compose up -d
```
## qBittorrent

### Overview
qBittorrent is an open-source torrent client that allows easy downloading of content with a lightweight web UI.

### Docker Compose Configuration
- File: `docker/qbittorrent/docker-compose.yml`
- Description: The Compose file sets up qBittorrent with the necessary networking and volume mappings for storage.

### Key Features
- Web-based torrent management
- Integration with VPN for secure downloading

### Usage
To start qBittorrent, navigate to its directory and run:
```
docker-compose up -d
```


