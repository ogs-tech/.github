# Alephee

> A **software engineering service** OGS provides under [OGS Partners](../) (Engineering):
> building and maintaining **Alephee**, a marketplace integration platform.

Alephee (the platform OGS builds for this engagement) lets vendors and platforms connect to
ecommerce marketplaces (Shopee, Bees, and others) through a standardized **adapter pattern**,
abstracting vendor-specific complexity behind canonical, URN-based data models.

- **Brand:** OGS Partners · Engineering *(service we provide)*
- **Repository:** [`ogs-tech/alephee`](https://github.com/ogs-tech/alephee) · folder `alephee/`
- **Shape:** meta-repo of six independent git repos cloned side by side
- **Authoritative docs:** [`alephee/docs/`](https://github.com/ogs-tech/alephee/tree/main/docs) — the repo's own Diátaxis portal. This hub frames Alephee in the OGS umbrella; the portal is the working source.

## Documentation (Diátaxis)

| | |
|---|---|
| 📚 [Tutorials](tutorials/) | Learn Alephee step by step |
| 🔧 [How-to guides](how-to/) | Accomplish specific tasks (onboard a vendor, run QA…) |
| 📖 [Reference](reference/) | The six sub-services, stacks, and commands |
| 💡 [Explanation](explanation/) | Architecture, the adapter pattern, URN identifiers |

## At a glance

| Sub-service | Purpose | Stack |
|---|---|---|
| **core-services** | Core microservices behind a Kong gateway (auth, catalogs, products, orders, pricing…) | NestJS · Lerna · MongoDB · Redis · Kong |
| **vendors-sdk** | Published SDK defining the adapter contract (`@alephee/vendors-adapter-sdk`) | NestJS lib · semantic-release · OpenAPI |
| **vendors-integration** | Concrete vendor adapters (Shopee, mocks) + shared vendor services | NestJS · Lerna · Kong |
| **vendors-bees-adapter** | Standalone adapter for the Bees platform | NestJS · MongoDB · BullMQ/Redis |
| **qa-automation** | E2E BDD regression suite (multi-client, Allure reports) | Java · Gradle · Selenium · Cucumber |
| **ui-core** | Shared React components + products front-end (`@alphee/ui-products`) | React 18 · Vite · MUI · TanStack Query |

> Deep docs live in the repo: the top-level [`alephee/docs/`](https://github.com/ogs-tech/alephee/tree/main/docs)
> portal, `alephee/ui-core/docs/` (front-end Diátaxis), and the SDK READMEs.
> This hub summarizes and links; it does not duplicate them.
