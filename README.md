# Final DevOps Project

## DevOps Setup

This project uses Docker Compose to run a React + Vite frontend, a .NET backend API, and an Nginx reverse proxy.

## Run locally

```bash
docker compose up --build -d
```

## URLs

Frontend:
http://localhost

Backend:
http://localhost/api/ping

## Services

- frontend: React + Vite frontend application
- backend: .NET backend API
- nginx: reverse proxy that routes traffic to frontend and backend

Only nginx exposes port 80 to the host machine.

## CI/CD Pipeline

The GitHub Actions pipeline automatically builds Docker images and deploys the application to the QA environment whenever code is pushed to the main branch.
