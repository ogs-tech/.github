# Noordhen — Reference

> *Information-oriented.* Sub-projects, stacks, commands, and environments.

## Sub-projects (in `noordhen/`)

### noordhen-react-app — Production front-end
- **Stack:** React 16, React Router 5, Bootstrap 4, Styled Components, Syncfusion Schedule
  (calendar), Draft.js (rich text), Axios
- **Commands:** `npm start`, `npm test`, `npm run build`

### noordhen-backup-nest-api — Backup automation service
- **Stack:** NestJS 10, Prisma 6, MySQL, node-ssh, mysqldump, Swagger/OpenAPI
- **Commands:** `yarn start`, `yarn start:dev`, `yarn test`, `yarn run build`

## Related external repositories

| Repo | Role | Stack |
|---|---|---|
| `noordhen-strapi-api` | Production backend | Strapi 3.1, MySQL |
| `noordhen-cprod-react-app` | CProd front-end | React 17 + TypeScript |
| `noordhen-cprod-strapi-api` | CProd backend | Strapi 3.6 |

## Environments & URLs

| Environment | URL |
|---|---|
| Production | `noordhen.com.br` |
| CProd (secondary) | `cprod.noordhen.com.br/auth` |
| CTop | `noordhen.com.br/ctop` |
| Central de Documentos | `noordhen.com.br/central-de-documentos` |

## Stack summary

- **Frontend:** React 16/17, TypeScript, Bootstrap 4/5, Styled Components
- **Backend:** Strapi 3 (Headless CMS), MySQL
- **Backup service:** NestJS 10, Prisma, MySQL, SSH
- **Runtime:** Node.js
