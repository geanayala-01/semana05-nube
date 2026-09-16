# Laboratorio 5 — Contenedores y Microservicios

Desarrollo de Soluciones en la Nube — Tecsup
Docente: Jaime Farfán

## Contenido

| Carpeta | Descripción |
|---|---|
| `lab-ejercicio1/` | Servidor Nginx con Docker Compose y bind mount |
| `lab-ejercicio2/` | App Node.js conectada a PostgreSQL vía red interna |
| `lab-ejercicio3/` | Persistencia de datos en MySQL con volúmenes nombrados |
| `lab-ejercicio4/` | Variables de entorno (`.env`) y healthchecks |

## Cómo ejecutar cada ejercicio

Entrar a la carpeta correspondiente y levantar los servicios:

```bash
cd lab-ejercicioN
docker compose up -d
docker compose ps
```

Para detener y limpiar:

```bash
docker compose down
```

> En `lab-ejercicio4/` se necesita un archivo `.env` (no incluido en el repo) con las variables `DB_USER`, `DB_PASS`, `DB_NAME`, `DB_PORT`, `APP_PORT` y `APP_ENV`.
