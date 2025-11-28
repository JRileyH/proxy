# Traefik Reverse Proxy with Auto SSL

Automatic HTTPS reverse proxy for hosting multiple Docker apps on different subdomains with automatic Let's Encrypt SSL certificates.

## Features

- Automatic HTTPS with Let's Encrypt
- Auto-discovery of Docker containers via labels
- Observability via Loki/Prometheus/Grafana

## Initial Setup

```bash
# SETUP SSH CRED STORAGE
touch acme.json
chmod 600 acme.json

# SETUP ENV VAR
touch .env
nano .env # (Paste your key from .env.example)

# SETUP DOCKER NETWORK / START
docker network create 
docker-compose up -d
```

