# Alephee — Reference

> *Information-oriented.* The six sub-services, their stacks, entry points, and how they relate.

Alephee is a **meta-repo**: six independent git repositories cloned side by side, each with its
own CI/CD and release cadence. Changes rarely span repos.

## Sub-services

### core-services
Core microservices powering integrations, API routing, and data aggregation (auth, catalogs,
products, orders, media, pricing, sales, publications, process monitoring) behind a Kong gateway.
- **Stack:** NestJS monorepo (Lerna + Yarn workspaces), Kong Gateway, MongoDB, Redis, Docker Compose
- **Commands:** `yarn build`, `yarn dev`
- **Local env:** `core-services/dev-compose.yaml` (Kong on 8000/8001/8444)
- **Role:** central hub; consumed by `ui-core` and `vendors-integration`; publishes events to vendors

### vendors-sdk
Published SDK (`@alephee/vendors-adapter-sdk`) defining the canonical adapter contract,
controllers, OpenAPI definition, and NestJS modules for vendor integrations.
- **Stack:** NestJS library, semantic-release (GitHub Packages), TypeScript, OpenAPI/Swagger
- **Commands:** `yarn build`, `yarn test`, `yarn test:e2e`
- **Release:** semantic-release on Conventional Commits — `feat`→minor, `fix`/`perf`→patch, `BREAKING CHANGE`→major
- **Role:** upstream dependency for `vendors-bees-adapter` and `vendors-integration`
- **Key docs:** `README.Adapters.md`, `README.OpenAPI.md`

### vendors-integration
Monorepo of concrete vendor adapter implementations (Shopee, mocks) and shared vendor-side
services (authentication, dispatcher, events, orders, products, publications, sales).
- **Stack:** NestJS monorepo (Lerna + Yarn workspaces), Kong Gateway
- **Commands:** `yarn build`, `yarn build:watch`; per-package `yarn test` in `packages/*`
- **Role:** consumes the SDK; deploys Kong-routed adapters that translate vendor APIs to canonical format

### vendors-bees-adapter
Standalone adapter implementation for the Bees platform; full lifecycle (auth, catalog,
listings, orders).
- **Stack:** NestJS, MongoDB (Mongoose + mongo-migrate-ts), BullMQ/Redis
- **Commands:** `yarn start:dev`, `yarn build`, `yarn migrations:up`, `yarn migrations:down`, `yarn test:e2e`
- **Role:** consumes `@alephee/vendors-adapter-sdk` + `@alephee/shared`; implements Categories, Listing, Media, Price, Stock, Orders, Invoices adapters

### qa-automation
End-to-end regression suite using BDD/Gherkin; multi-client config (demo, cliente2, default)
with tag-driven runs and Allure reporting.
- **Stack:** Java (JDK 17), Gradle, Selenium WebDriver, Cucumber/Gherkin, TestNG, Allure, Page Object Model
- **Commands:** `./gradlew cucumber`, `./gradlew cucumber -Dclient=demo`, `./gradlew allureReport`
- **Role:** validates flows across core-services, ui-core, and vendor integrations; reports publish to GitHub Pages nightly

### ui-core
Shared React component library and products front-end (`@alphee/ui-products`); catalogs,
publications, pricing, stock uploads with bulk import flows.
- **Stack:** React 18 + TypeScript (strict) + Vite (SWC), MUI v5 + Tailwind, TanStack Query v4, Formik/Yup, i18next
- **Commands:** `yarn dev` (proxies `/api` → `gateway-test.alephee.com`), `yarn build`, `yarn lint`
- **Locales:** en-US, es-AR, pt-BR · **Path alias:** `@this/*` → `src/*`
- **Tests:** none — verify in browser
- **Docs:** `ui-core/docs/` — full Diátaxis portal (the authoritative source)

## Cross-cutting reference

| Concept | Where | Note |
|---|---|---|
| GitHub Packages auth | `.npmrc` | PAT with `read:packages` for `@alephee/*` deps |
| URN identifiers | `UrnUtil` (vendors-sdk) | construct/parse canonical IDs consistently |
| `AlepheeNestJsModule` | all NestJS services | wires Swagger, logging, correlation IDs, exception filters |
| `@this/*` alias | tsconfig + module aliases | keep Vite config in sync |

## Source files

- Meta-repo guide: `alephee/CLAUDE.md`
- `alephee/core-services/README.md` · `alephee/vendors-sdk/README.md` (+ Adapters/OpenAPI)
- `alephee/vendors-integration/README.md` · `alephee/vendors-bees-adapter/README.md`
- `alephee/qa-automation/CLAUDE.md` · `alephee/ui-core/docs/README.md`
