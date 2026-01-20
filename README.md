# FastAPI CI/CD Project

API FastAPI con integración y despliegue continuo en GCP Cloud Run.

## Descripción

Este proyecto implementa una API simple con FastAPI que se despliega automáticamente en GCP Cloud Run mediante GitHub Actions.

## Requisitos

- Python 3.12+
- Poetry
- Docker
- Cuenta de GCP

## Instalación local

```bash
poetry install
poetry run uvicorn app.main:app --reload
```

## Docker

```bash
docker build -t fastapi-app .
docker run -p 8000:8000 -e PORT=8000 fastapi-app
```
