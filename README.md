# Learning Management Service — Secure API

A backend API for a learning management system with authentication, database integration, and hardened deployment.

## Features

- REST API with Swagger/OpenAPI documentation
- API key authentication
- PostgreSQL database integration
- `/interactions` and `/learners` endpoints
- Hardened Linux VM deployment (firewall, fail2ban, SSH hardening)

## Tech stack

- Python 3.12+, FastAPI
- PostgreSQL, pgAdmin
- pytest, HTTP client testing
- Docker, Docker Compose
- Linux hardening tools

## Quick start

```bash
# Copy environment files
cp .env.example .env
cp .env.docker.example .env.docker.secret

# Run with Docker Compose
docker compose up --build
```

## Project structure

- `src/app/` — FastAPI backend
- `tests/` — unit and integration tests
- `docker-compose.yml` — backend + postgres + pgAdmin
