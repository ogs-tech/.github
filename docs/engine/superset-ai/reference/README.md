# Superset AI — Reference

<!-- nav -->
[Docs](../../../) › [OGS Engine](../../) › [Superset AI](../) › Reference

> *Information-oriented.* The app, its stack, and commands.

## Superset AI App — `superset-ai-app` (single developer)

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

## Source files

- [`ogs-tech/superset-ai-app`](https://github.com/ogs-tech/superset-ai-app): `README.md`, [`docs/`](https://github.com/ogs-tech/superset-ai-app/tree/main/docs) — the repo's own Diátaxis portal (authoritative)

---

📚 [Tutorials](../tutorials/) · 🔧 [How-to](../how-to/) · 📖 Reference · 💡 [Explanation](../explanation/)
↑ [Superset AI](../) · [Docs Hub](../../../)
