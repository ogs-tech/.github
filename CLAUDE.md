# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is the **OGS Tech** GitHub organization's special `.github` repository. It controls the org's public presence on GitHub.

- `profile/README.md` — renders as the organization's public profile on the OGS Tech GitHub org page
- `README.md` — repository-level description

## Key Files

| File | Purpose |
|---|---|
| `profile/README.md` | Public org profile — visible to everyone on GitHub |
| `README.md` | Repo description and roadmap |
| `docs/` | Org-wide documentation hub — brand umbrella + Diátaxis per product (see below) |

## Documentation Hub (`docs/`)

`docs/` is the organization-wide documentation, organized by the **brand umbrella**, not by folder:

- **`docs/explanation/`** — the umbrella itself: [`brand-architecture.md`](docs/explanation/brand-architecture.md), `how-it-connects.md`, `glossary.md`
- **`docs/partners/`** — OGS Partners (Alephee, Noordhen)
- **`docs/studio/`** — OGS Studio (Press, Co., Royale IQ)
- **`docs/engine/`** — OGS Engine (Press CMS core, Agent AI, Superset AI)

Each product has the four [Diátaxis](https://diataxis.fr) quadrants (`tutorials/`, `how-to/`,
`reference/`, `explanation/`). Conventions:

- **Language: English.**
- **One home per codebase:** Engine holds *technical* reference; Studio holds *product / GTM* framing; they cross-link instead of duplicating.
- **Link, don't duplicate:** if a repo already has docs (e.g. `alephee/ui-core/docs/`, `sde-superset-ai-app/docs/`), link to them from `reference/`.
- **`_legacy/` is intentionally not documented.**
- When adding a new project, place it under its brand and follow the Diátaxis quadrant structure.

## Guidelines

- **Markdown only** — no build steps, no dependencies, no CI pipelines currently
- Changes to `profile/README.md` are **immediately visible** on the public GitHub org page — review carefully before committing
- Keep `profile/README.md` concise and aligned with OGS Tech's mission: SaaS, AI/autonomous agents, and open source

## Roadmap (planned additions)

This repo may eventually centralize:
- Reusable GitHub Actions workflows (`.github/workflows/`)
- Issue and pull request templates (`.github/ISSUE_TEMPLATE/`, `.github/PULL_REQUEST_TEMPLATE.md`)
- Organization-wide default settings
