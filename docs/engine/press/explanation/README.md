# Press (CMS core) — Explanation

<!-- nav -->
[Docs](../../../) › [OGS Engine](../../) › [Press](../) › Explanation

> *Understanding-oriented.* Why the Press engine exists and how it becomes a product.

## Why a scaffolder, not a framework

Agencies and developers rebuild the same content-site plumbing over and over: a headless CMS, a
front-end, shared types, and dynamic content blocks. Press packages that plumbing into a **one
command** so a production-ready monorepo exists in minutes — opinionated defaults, pinned
versions, no wiring by hand.

## Pinned versions, coordinated upgrades

The generated stack pins **major versions** so that every site scaffolded from Press can be
upgraded together. This is a deliberate trade-off: less per-project freedom in exchange for a
fleet you can maintain centrally — essential for the Studio "Cloud" and "Co." doors where OGS
operates many sites.

## The engine → product path

Press is an **engine** in OGS Engine. It graduates into the **OGS Studio Press** product, sold
through three doors:

| Door | Buyer | Model |
|---|---|---|
| Open Source | developers | free, self-host (this is **NIS / `@nis/create`**) |
| Cloud | agencies | managed, paid → [studio-press-cloud](../../../studio/press/) |
| Co. | SMBs | done-for-you, operated by [Studio Co.](../../../studio/co/) |

The same core engine serves all three; only the packaging and who operates it changes. See
[How it connects](../../../explanation/how-it-connects.md).

---

📚 [Tutorials](../tutorials/) · 🔧 [How-to](../how-to/) · 📖 [Reference](../reference/) · 💡 Explanation
↑ [Press](../) · [Docs Hub](../../../)
