# Superset AI — Explanation

> *Understanding-oriented.* Why Superset AI exists.

## The problem

AI coding assistants (Claude Code, Copilot, Codex) each want their customizations — skills,
references, agent profiles, instructions — in their own place and format. Keeping these in sync by
hand, or scattered across Notion and loose files, doesn't scale. Superset AI makes a **single
source of truth** in Markdown + YAML and projects it into each assistant.

## Local-first, Markdown + YAML

Artifacts are plain **Markdown + YAML**: diffable, git-versioned, and editable without the app.
The app is **local-first** — no backend, no API, no telemetry. It syncs to assistants via
**symbolic links**, so edits in one place appear everywhere instantly.

## Why it stays internal

Unlike Press and Agent AI, Superset AI does **not** graduate into a Studio product — it is the
team's own leverage for working effectively with Claude and other assistants. See
[Brand Architecture](../../../explanation/brand-architecture.md).
