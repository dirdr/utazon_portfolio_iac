# Utazon Portfolio Infrastructure 🏗️

## About 🤔

This repository contains the IaC for deploying the Utazon portfolio website on a VPS using Traefik as a reverse proxy.

The deployment target is a custom Traefik configuration - you can find the complete setup [here](https://github.com/dirdr/homelab_config).

## Prerequisites 📋

Before you start, make sure you have:
- Docker and Docker Compose installed 🐳
- Access to a VPS with Traefik already configured
- The target configuration repository cloned

## Getting Started 🚀

1. Clone the repositories
2. Start your Traefik stack
3. Configure environment variables
Create a `.env` file for your chosen environment and populate it with the required values:

```bash
cp .env.example .env
# Edit .env with your specific values
```

### 4. Deploy the application
```bash
sudo docker compose up -d
```

## Environment Variables 🔧

Check the `.env.example` file for all required environment variables. The main one you'll need is:

- `UTAZON_DOMAIN_<ENV>: The domain where the application will be accessible
