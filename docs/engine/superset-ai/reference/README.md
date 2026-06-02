# Superset AI — Reference

> *Information-oriented.* The two apps, their stacks, and commands.

## Skillforge — `sde-ai-app` (single developer)

Desktop app that centralizes AI customizations (skills, references, agent profiles, global
instructions) as Markdown + YAML, then syncs them to Claude Code and GitHub Copilot via
**symbolic links**.

- **Stack:** Electron 41, React 19, TypeScript 5.9, MUI, Emotion; build with electron-vite + Vite 7;
  tests with Vitest + Testing Library; validation with Zod
- **Architecture:** local-first — no backend, no API, no telemetry
- **Commands:**
  | Command | Purpose |
  |---|---|
  | `npm run dev` | Electron + Vite HMR |
  | `npm run build` | Production build to `out/` |
  | `npm test` / `npm run test:watch` | Vitest (node + jsdom projects) |
  | `npm run lint` / `npm run typecheck` / `npm run format` | Quality gates |
- **Status:** Spike — single-developer dogfooding, time-boxed. See `docs/explanation/prd.md` for
  goals and stop rules. In-repo docs follow Diátaxis.

## Specfy — `company-ai-app` (team)

Sibling of Skillforge for engineering teams (5–20 devs): manage a centralized `company-context`
repo of skills, references, and AI agent profiles; export to Claude Code, GitHub Copilot, and
OpenAI Codex.

- **Stack:** TBD (likely Electron + React, mirroring Skillforge). Local-first, git-based
  collaboration, no backend.
- **Commands:** TBD (discovery phase)
- **Status:** Discovery — PRD only; `ARCH.md` and `ROADMAP.md` to be created
- **Validation:** 1 company-pilot for ≥8 weeks, ≥10 skills published, ≥3 devs actively consuming via
  export, without regressing to Notion/loose files

## Source files

- `internal/sde-ai-app/README.md`, `CLAUDE.md`, `docs/` (Diátaxis)
- `internal/company-ai-app/README.md`, PRD
