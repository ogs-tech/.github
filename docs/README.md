# OGS Tech — Documentation Hub

**English** · [Português](README.pt-BR.md)

> **Technology that takes your business further.** · *Future Ready.*

This is the organization-wide documentation hub for **OGS Tech** (Odenir Gomes Solutions).
It is organized around the **brand umbrella** — how the business packages, sells, and operates.
Detailed product docs live in each repository; this hub frames them and links out.

- **Brand-first:** docs are grouped by brand (Partners, Studio, Engine), not by folder.
- **Link, don't duplicate:** product docs (tutorials, how-to, reference, architecture) live in
  each repo. This hub frames each product and links out — it does **not** copy them.
- **Hub, not silo:** what lives here is genuinely org-wide — the brand umbrella, the
  cross-brand explanation, and a one-page frame per product.

---

## The umbrella at a glance

```
OGS Tech (Odenir Gomes Solutions)
│
├── OGS Partners ........... premium · bespoke · high-margin · useogs.com/partners
│     ├── Engineering ...... Alephee
│     └── Support .......... Noordhen
│
├── OGS Studio ............. scalable · packages & sells · useogs.com/studio
│     ├── Press ............ Open Source (devs · self-host) / Cloud (agencies · managed)
│     ├── Co. ............. IT services for Brazilian SMBs (done-for-you, runs the Press)
│     └── Royale IQ ........ influencers niche · pro bono
│
└── OGS Engine ............ the machine room · builds the technology
      ├── Press ........... CMS core   → becomes OGS Studio Press
      ├── Agent AI ........ AI core    → becomes the Royale IQ app
      └── Superset AI ..... internal desktop tool (helps the team use Claude)
```

See [Brand Architecture](explanation/brand-architecture.md) for the full picture and
[How it connects](explanation/how-it-connects.md) for the flow between brands.
For the brand *identity* — mission, values, logo, color, typography — see [Brand](brand/).

---

## Navigate by brand

### 🤝 [OGS Partners](partners/) — *premium, bespoke*
| Product | What it is | Docs |
|---|---|---|
| [Alephee](partners/alephee/) | Marketplace integration platform (engineering partner) | [repo docs ↗](https://github.com/ogs-tech/alephee/tree/main/docs) |
| [Noordhen](partners/noordhen/) | Custom operations platform for Noordhen Brasil (support partner) | [repo docs ↗](https://github.com/ogs-tech/noordhen/tree/main/docs) |

### 🏭 [OGS Studio](studio/) — *scalable, packaged*
| Product | What it is | Docs |
|---|---|---|
| [Press](studio/press/) | Content-site platform — three doors over one engine | [product](studio/press/) |
| [Press Cloud](studio/press-cloud/) | Managed multi-tenant Press SaaS (the Cloud door) | [product](studio/press-cloud/) |
| [Co.](studio/co/) | Done-for-you IT services for SMBs | [product](studio/co/) |
| [Royale IQ](studio/royale-iq/) | AI coach for Clash Royale players (pro bono) | [product](studio/royale-iq/) |

### ⚙️ [OGS Engine](engine/) — *the machine room*
| Engine | What it is | Repo |
|---|---|---|
| [Press](engine/press/) | CMS core (`@nis/create` scaffolder) | [studio-press-cli ↗](https://github.com/ogs-tech/studio-press-cli) |
| [Agent AI](engine/agent-ai/) | AI core powering Royale IQ | [royale-agent-ai-app ↗](https://github.com/ogs-tech/royale-agent-ai-app) |
| [Superset AI](engine/superset-ai/) | Internal Claude-tooling desktop apps | [superset-ai-app ↗](https://github.com/ogs-tech/superset-ai-app) |

---

## Planning & boards

Day-to-day planning runs on **Trello**. Two boards mirror the brand umbrella:

| Board | Scope |
|---|---|
| [OGS Tech HQ](https://trello.com/b/JpvCIoWc/ogs-tech-hq) | Organization-wide — brands, GTM, operations |
| [OGS Tech Engine](https://trello.com/b/3lPid3OR/ogs-tech-engine) | The machine room — engineering & product execution |

> Access is restricted to the OGS team. These boards are the source of truth for *work in
> progress*; this hub documents the *stable* picture.

---

## Conventions for contributors

- **Language:** English.
- **One home per codebase:** a repo is documented once under its primary brand. Engine holds
  the *technical* framing; Studio holds the *product / go-to-market* framing and cross-links.
- **Link, don't duplicate:** detailed docs live in each repo — the product page here links to
  them, it does not copy them.
- **Markdown only:** no build step, no dependencies (see [CLAUDE.md](../CLAUDE.md)).

---

*Odenir Gomes Solutions (OGS) · CNPJ 54.705.657/0001-83 · São Paulo/SP · founded 2024-04-12*
*[ogsolucoes.com.br](https://ogsolucoes.com.br)*
