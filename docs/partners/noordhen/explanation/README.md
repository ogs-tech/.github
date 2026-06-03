# Noordhen — Explanation

> *Understanding-oriented.* Why Noordhen is built the way it is.

## A bespoke platform for one client

Noordhen is a **Support** engagement: OGS maintains a custom operations platform for Noordhen
Brasil. It is not a productized offering — it is tailored to one organization's operations
(scheduling, documents, team communication).

## The Production / CProd split

The platform runs as **two parallel environments**:

- **Production** (`noordhen.com.br`) — the live system used by the business.
- **CProd** (`cprod.noordhen.com.br`) — a secondary instance, with its own front-end and Strapi
  backend (`noordhen-cprod-*`), used to validate changes against production-like data before they
  reach the live environment.

Each environment has its own React app and Strapi API, so the two can evolve and be deployed
independently.

## Why Strapi + MySQL

The content and operational data are modeled in **Strapi 3.x** (headless CMS) over **MySQL**, which
gives non-developers an admin UI to manage records while the React front-ends consume the API.

## Why a separate backup service

`noordhen-backup-nest-api` is a dedicated NestJS service that automates database backups over SSH
(`mysqldump` + `node-ssh`), keeping backup logic out of the application backends and giving it its
own schedule, API, and Prisma-managed metadata.

See [Reference](../reference/) for stacks, commands, and environment URLs.
