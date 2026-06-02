# Superset AI — Explanation

> *Understanding-oriented.* Why Superset AI exists and why there are two apps.

## The problem

AI coding assistants (Claude Code, Copilot, Codex) each want their customizations — skills,
references, agent profiles, instructions — in their own place and format. Keeping these in sync by
hand, or scattered across Notion and loose files, doesn't scale. Superset AI makes a **single
source of truth** in Markdown + YAML and projects it into each assistant.

## Local-first, Markdown + YAML

Artifacts are plain **Markdown + YAML**: diffable, git-versioned, and editable without the app.
The apps are **local-first** — no backend, no API, no telemetry. Skillforge syncs to assistants via
**symbolic links**, so edits in one place appear everywhere instantly.

## Why two apps

| App | Audience | Why separate |
|---|---|---|
| **Skillforge** (`sde-superset-ai-app`) | one developer | fast personal dogfooding; spike with explicit stop rules |
| **Specfy** (`company-superset-ai-app`) | a team (5–20 devs) | git-based collaboration on a shared `company-context`; exports to more assistants (adds Codex) |

Skillforge validates the single-user idea before Specfy invests in the team workflow.

## Why it stays internal

Unlike Press and Agent AI, Superset AI does **not** graduate into a Studio product — it is the
team's own leverage for working effectively with Claude and other assistants. See
[Brand Architecture](../../../explanation/brand-architecture.md).
