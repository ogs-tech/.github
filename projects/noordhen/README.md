# Noordhen

Platform for managing operations, scheduling, documents, and team communication — built for small and medium businesses.

---

## Architecture Overview

Noordhen is composed of two independent environments sharing the same product domain:

| Environment | Purpose |
|---|---|
| **Production** | Main environment — stable, client-facing |
| **CProd** | Secondary instance — parallel deployment |

Each environment has its own frontend and backend:

| Layer | Production | CProd |
|---|---|---|
| Frontend | `noordhen-react-app` | `noordhen-cprod-react-app` |
| Backend (CMS/API) | `noordhen-strapi-api` | `noordhen-cprod-strapi-api` |

A dedicated backup service handles automated database backups across both environments:

| Service | Repo |
|---|---|
| Backup API | `noordhen-backup-nest-api` |

---

## Repositories

### [`noordhen-react-app`](https://github.com/ogs-tech/noordhen-react-app)

**Production frontend** — React 16 application (JavaScript).

- React 16 + React Router 5
- Bootstrap 4 + Styled Components
- Syncfusion Schedule (calendar/scheduling)
- Draft.js (rich text editor)
- Axios for API communication

---

### [`noordhen-strapi-api`](https://github.com/ogs-tech/noordhen-strapi-api)

**Production backend** — Strapi 3 headless CMS with MySQL.

- Strapi 3.1 (content management)
- MySQL via Bookshelf/Knex
- Nodemailer (email notifications)
- Strapi built-in: users/permissions, upload, documentation

---

### [`noordhen-cprod-react-app`](https://github.com/ogs-tech/noordhen-cprod-react-app)

**CProd frontend** — React 17 application (TypeScript).

- React 17 + TypeScript + React Router 5
- Bootstrap 5 + Styled Components
- Datatables.net (data grids)
- SweetAlert 2 (user feedback)
- Axios for API communication

---

### [`noordhen-cprod-strapi-api`](https://github.com/ogs-tech/noordhen-cprod-strapi-api)

**CProd backend** — Strapi 3.6 headless CMS with MySQL.

- Strapi 3.6 (latest 3.x — includes i18n)
- MySQL via Bookshelf/Knex
- SQLite3 for local development
- Nodemailer (email notifications)

---

### [`noordhen-backup-nest-api`](https://github.com/ogs-tech/noordhen-backup-nest-api)

**Backup service** — NestJS API for automated database backup management.

- NestJS 10 + TypeScript
- Prisma 6 (ORM)
- `@nestjs/schedule` (cron jobs)
- `node-ssh` (remote SSH connection)
- `mysqldump` (database export)
- Swagger/OpenAPI documentation

---

## Tech Stack Summary

| Layer | Technologies |
|---|---|
| Frontend | React 16/17, TypeScript, Bootstrap 4/5, Styled Components |
| Backend | Strapi 3 (Headless CMS), MySQL |
| Backup Service | NestJS 10, Prisma, MySQL, SSH |
| Runtime | Node.js |

---

## Environments & URLs

| Environment | URL |
|---|---|
| Production | [noordhen.com.br](https://noordhen.com.br) |
| CProd | [cprod.noordhen.com.br/auth](https://cprod.noordhen.com.br/auth) |
| CTop | [noordhen.com.br/ctop](https://noordhen.com.br/ctop) |
| Inputs 360 / Central de Documentos | [noordhen.com.br/central-de-documentos](https://noordhen.com.br/central-de-documentos) |

---

## Project Status

> Active — maintained by [OGS Tech](https://github.com/ogs-tech)
