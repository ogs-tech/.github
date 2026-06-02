# Alephee — Explanation

> *Understanding-oriented.* Why Alephee is built the way it is.

## The engagement

Alephee is an **OGS Partners · Engineering** engagement: OGS provides software engineering as a
service, and the deliverable is the marketplace integration platform described below. The
architecture choices here are OGS's, made to deliver that service well.

## The problem

Every marketplace (Shopee, Bees, …) exposes a different API, different identifiers, and a
different lifecycle for catalogs, listings, orders, and invoices. Integrating each one ad hoc
creates N×M complexity. Alephee collapses that into a **canonical model + adapter pattern**.

## Core ideas

### Canonical model with URN identifiers
Entities are addressed by **URNs** (Uniform Resource Names) so the same product/order can be
looked up consistently across systems. IDs are constructed and parsed via `UrnUtil` (in
`vendors-sdk`) rather than by ad-hoc string building.

### The adapter pattern
`vendors-sdk` defines abstract adapters — Categories, Listing, Media, Price, Stock, Orders,
Invoices, Auth. Concrete adapters (`vendors-bees-adapter`, Shopee in `vendors-integration`)
implement those contracts, translating vendor APIs into the canonical format. New marketplaces
become "just another adapter."

### Meta-repo, not monorepo
Six independent git repos are cloned side by side. Each ships, versions, and releases on its own
cadence; cross-repo changes are rare. The SDK is the shared contract that holds them together —
published to GitHub Packages and consumed as `@alephee/vendors-adapter-sdk`.

### Gateway-fronted microservices
Kong sits in front of the services (ports 8000/8001/8444). `core-services` is the hub; `ui-core`
and the vendor adapters talk to it. Events flow out to vendor adapters.

### Shared NestJS wiring
`AlepheeNestJsModule` globally wires Swagger, structured logging, correlation IDs, and exception
filters — so individual services don't re-implement cross-cutting concerns (don't manually add
`@UseFilters` when it's present).

## Trade-offs

- **Meta-repo** keeps services decoupled and independently releasable, at the cost of no atomic
  cross-service commits — the SDK contract absorbs that coordination.
- **ui-core has no unit tests** — verification is done in the browser; reference flows live in its
  own Diátaxis docs.

See [Reference](../reference/) for concrete commands and per-service details.
