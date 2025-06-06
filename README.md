# Nuxt + Nest Template

This repository provides a simple template for a web application using **Nuxt.js** for the frontend and **Nest.js** for the backend. The environment runs on Docker and uses **PostgreSQL** with **Prisma** for database access.

## Structure

- `frontend` - Nuxt 3 application
- `backend` - Nest application with Prisma
- `docker-compose.yml` - launches frontend, backend and PostgreSQL services

## Usage

1. Build and start all services:
   ```bash
   docker-compose up --build
   ```
2. Access the frontend at `http://localhost:3000` and the backend API at `http://localhost:3001`.

The backend connects to PostgreSQL using the connection information defined in `docker-compose.yml`. Prisma schema and a simple seed script are provided under `backend/prisma`.
