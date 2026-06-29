# Chapter 8 — Deploying Agents as APIs
### FastAPI, Celery, Redis, Docker, and Cloud Deployment

## Files
chapter8/

├── api/

│   ├── main.py           ← FastAPI app

│   ├── routes.py         ← Agent endpoints

│   ├── auth.py           ← API key + JWT auth

│   └── cost_control.py   ← Budget protection

├── worker/

│   ├── celery_app.py     ← Celery worker

│   └── tasks.py          ← Async agent tasks

├── Dockerfile            ← Container setup

├── docker-compose.yml    ← Full stack

└── .github/workflows/

└── deploy.yml        ← CI/CD pipeline

## What You Learn
- FastAPI request lifecycle for agents
- Async job queue (Celery + Redis)
- API key and JWT authentication
- Three-layer cost protection
- Docker containerisation
- Cloud deployment (Railway / Fly.io)
- Observability stack

## Setup
```bash
pip install fastapi uvicorn celery redis httpx
docker-compose up --build
```

## Endpoints
POST /api/v1/agent/run     ← Submit agent job

GET  /api/v1/runs/{id}     ← Check job status

GET  /api/v1/runs/{id}/result ← Get result

