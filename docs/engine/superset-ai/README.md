# Superset AI — internal tooling *(OGS Engine)*

> Desktop tooling that **helps the OGS team use Claude** and its adaptations. Internal use only —
> it does **not** graduate into a sold product.

Superset AI centralizes AI customizations (skills, references, agent profiles, global
instructions) as Markdown + YAML and syncs them to AI coding assistants. It has two
implementations: a single-developer app and a team app.

- **Brand:** OGS Engine · internal tool
- **Repositories:**
  - [`ogs-tech/sde-superset-ai-app`](https://github.com/ogs-tech/sde-superset-ai-app) — **Skillforge** (single developer) · folder `internal/sde-superset-ai-app`
  - [`ogs-tech/company-superset-ai-app`](https://github.com/ogs-tech/company-superset-ai-app) — **Specfy** (team) · folder `internal/company-superset-ai-app`

## Documentation (Diátaxis)

| | |
|---|---|
| 📚 [Tutorials](tutorials/) | Set up and sync your AI artifacts |
| 🔧 [How-to guides](how-to/) | Add a skill, export to an assistant |
| 📖 [Reference](reference/) | Both apps, stacks, commands |
| 💡 [Explanation](explanation/) | Local-first, Markdown+YAML, why two apps |

## At a glance

| App | Scope | Stack | Status |
|---|---|---|---|
| **Skillforge** (`sde-superset-ai-app`) | single developer | Electron 41 · React 19 · MUI · Vitest · Zod | Spike (dogfooding) |
| **Specfy** (`company-superset-ai-app`) | team (5–20 devs) | likely Electron + React (mirrors Skillforge) | Discovery (PRD only) |
