# Agent AI — Reference

> *Information-oriented.* Monorepo layout, stacks, and commands for `royale-agent-ai-app`.

## Monorepo

A **Turborepo + pnpm** monorepo combining a serverless backend with a mobile-first front-end and
shared TypeScript contracts.

| Package | Role | Stack |
|---|---|---|
| `@royale-agent-app/app` | Front-end (mobile-first) | React 18, Ionic 8, Capacitor 6 |
| `@royale-agent-app/functions` | Serverless backend | AWS Lambda, Serverless Framework, LangGraph |
| shared | Type contracts | TypeScript |

## Commands

| Command | Purpose |
|---|---|
| `pnpm install` | Install dependencies |
| `pnpm dev` | Start all services in dev mode |
| `pnpm --filter @royale-agent-app/functions dev` | Backend only |
| `pnpm --filter @royale-agent-app/app dev` | Front-end only |
| `pnpm build` / `pnpm lint` / `pnpm test` | Build / lint / test |

## Status & docs

- **Phase:** Active development
- **In-repo docs:** `./.specify/docs/` (index, architecture, integrations, operations)

## Source files

- `internal/royale-agent-ai-app/README.md`, `CLAUDE.md`, `./.specify/docs/`
