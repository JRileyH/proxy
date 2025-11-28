# Traefik Reverse Proxy with Auto SSL

Automatic HTTPS reverse proxy for hosting multiple Docker apps on different subdomains with automatic Let's Encrypt SSL certificates.

## Features

- Automatic HTTPS with Let's Encrypt
- Auto-discovery of Docker containers via labels
- HTTP to HTTPS redirect
- Multiple subdomains support
- Simple docker-compose label configuration

## Initial Setup

```bash
# If it exists
sudo rm -rf acme.json

touch acme.json
chmod 600 acme.json

touch .env
nano .env # (Paste your key from .env.example)

docker network create 
docker-compose up -d
```

