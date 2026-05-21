# Taller DevOps Monorepo Dockerizado

Este repositorio es una versión dockerizada de los proyectos:
- `Taller-DevOps-API-REST`
- `Taller-DevOps-Front`

El objetivo es ejecutar la aplicación completa (backend y frontend) usando Docker Compose, sin tener que instalar dependencias locales en la máquina.

## Estructura del proyecto

- `backend/` - Código del API REST.
- `frontend/` - Código de la aplicación web.
- `docker-compose.yml` - Orquesta los servicios de backend y frontend.

## Requisitos

- Docker
- Docker Compose

## Ejecución

Desde la raíz del repositorio, ejecuta:

```bash
docker compose up --build
```

Esto levantará los contenedores necesarios para el backend y el frontend.

## Acceso
 
* http://localhost:3000

## Notas

- Si ya existe una versión en ejecución, utiliza `docker compose down` antes de levantar los servicios de nuevo.
- Si necesitas reconstruir los contenedores sin cache:

```bash
docker compose build --no-cache
```


