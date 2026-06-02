# Press (CMS core) — Reference

> *Information-oriented.* The `@nis/create` CLI and what it generates.

## CLI

| Item | Value |
|---|---|
| Package | `@nis/create` |
| Invocation | `@nis/create` (generator CLI) |
| Goal | Scaffold a production-ready full-stack content-site monorepo in ≤2 min |
| Repo | `internal/cloud-press-cli` |

## Generated monorepo

The generator produces an opinionated **Turborepo-style** monorepo:

- a **front-end app**
- a **CMS app** (headless)
- **shared packages** (type-sharing between CMS and front-end)
- **dynamic blocks** wired end to end

> Exact framework, headless CMS, and type-sharing pattern are defined in the repo's `ARCH.md`,
> with **pinned major versions** to enable coordinated upgrades. Treat `ARCH.md` as the source
> of truth and mirror version changes here.

## Status & validation targets

- **Phase:** Discovery (PRD + `ARCH.md` present)
- **Validation (post-`v0.1`, 3 months):** ≥20 external PRs, ≥100 installs, ≥1 agency fork/rebrand

## Source files

- `internal/cloud-press-cli/README.md`, `PRD`, `ARCH.md`
