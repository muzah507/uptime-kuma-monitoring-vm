# Docker Setup

This document explains how to install Docker and deploy Uptime Kuma.

---

# Install Docker

## Update Repository

```bash
sudo apt update
```
```bash
sudo apt install docker.io docker-compose -y
```
# Enable Docker Service
```bash
sudo systemctl enable docker
sudo systemctl start docker
```
# Clone Repository
```bash
git clone https://github.com/yourusername/uptime-kuma-monitoring-vm.git
```
Enter project directory:
```bash
cd uptime-kuma-monitoring-vm
```
# Deploy Uptime Kuma
```bash
cd configs
```
Run Docker Compose:
```bash
docker compose up -d
```

# Docker Compose File
```YAML
services:
  uptime-kuma:
    image: louislam/uptime-kuma:1
    container_name: uptime-kuma
    restart: always

    ports:
      - "3001:3001"

    volumes:
      - uptime-kuma:/app/data

    environment:
      - TZ=Asia/Jakarta

volumes:
  uptime-kuma:
```
