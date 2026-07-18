# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is the **OGS tech** GitHub organization's special `.github` repository. It controls the org's public presence on GitHub.

- `profile/README.md` — renders as the organization's public profile on the OGS tech GitHub org page
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
- **`docs/brand/`** — brand identity from the Guia de Marca, Ed. 03: `company.md` (mission/vision/values), `visual-identity.md` (logo, color, type)
- **`docs/partners/`** — OGS Partners (Alephee, Noordhen)
- **`docs/studio/`** — OGS Studio (Press, Co., Royale IQ)
- **`docs/engine/`** — OGS Engine (Press CMS core, Agent AI, Superset AI)

Each product is a **single `README.md`** that frames the product in the umbrella and links out to
its repo. The hub deliberately does **not** carry per-product Diátaxis quadrants
(`tutorials/`, `how-to/`, `reference/`, `explanation/`) — that detail lives in each project's repo
and would only be duplicated here. The four quadrants live inside the repos, not in this hub.
Conventions:

- **Language: English.** (`README.pt-BR.md` translates the main hub pages.)
- **One home per codebase:** Engine holds the *technical* framing; Studio holds the *product / GTM* framing; they cross-link instead of duplicating.
- **Link, don't duplicate:** detailed docs (tutorials, how-to, reference, architecture) live in
  each repo (e.g. `alephee/docs/`, `noordhen/docs/`, `studio-press-cli`). The product page links
  to them — it does not copy them.
- **What does live here:** `docs/brand/` (identity) and `docs/explanation/` (the cross-brand
  umbrella) — both genuinely org-wide and not duplicated in any repo.
- **`_legacy/` is intentionally not documented.**
- When adding a new project, place it under its brand as a single framing `README.md` that links to its repo.

## Guidelines

- **Markdown only** — no build steps, no dependencies, no CI pipelines currently
- Changes to `profile/README.md` are **immediately visible** on the public GitHub org page — review carefully before committing
- Keep `profile/README.md` concise and aligned with OGS tech's mission: SaaS, AI/autonomous agents, and open source

## Roadmap (planned additions)

This repo may eventually centralize:
- Reusable GitHub Actions workflows (`.github/workflows/`)
- Issue and pull request templates (`.github/ISSUE_TEMPLATE/`, `.github/PULL_REQUEST_TEMPLATE.md`)
- Organization-wide default settings
