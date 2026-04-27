# Sistema de Precios de Cacao

Aplicación web full-stack para registrar y consultar los precios del cacao.

## URLs desplegadas

- **Frontend:** https://reto-cacao-frontend.vercel.app
- **Backend:** https://reto-cacao-backend-production.up.railway.app
- **Documentación API:** https://reto-cacao-backend-production.up.railway.app/docs

## Stack tecnológico

| Capa | Tecnología |
|---|---|
| Frontend | Angular 21 + Tailwind CSS |
| Backend | FastAPI (Python) |
| Base de datos | PostgreSQL |
| Gestor de paquetes Python | uv |
| Despliegue frontend | Vercel |
| Despliegue backend | Railway |

## Correr el backend localmente con Docker

```bash
docker build -t reto-cacao-backend .
docker run -p 8000:8000 --env-file .env reto-cacao-backend
```

## Correr el backend localmente con uv

```bash
cd backend
uv venv
source .venv/bin/activate
uv run uvicorn app.main:app --reload
```

## Variables de entorno

Crea un archivo `.env` basado en `.env.example`: