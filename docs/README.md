# OGS Tech — Documentation Hub

**English** · [Português](README.pt-BR.md)

> **Technology that takes your business further.** · *Future Ready.*

This is the organization-wide documentation hub for **OGS Tech** (Odenir Gomes Solutions).
It is organized around the **brand umbrella** — how the business packages, sells, and
operates — and follows the [Diátaxis](https://diataxis.fr) framework within each product.

- **Brand-first:** docs are grouped by brand (Partners, Studio, Engine), not by folder.
- **Diátaxis-within:** every product has *Tutorials*, *How-to guides*, *Reference*, and *Explanation*.
- **Hub, not silo:** this hub holds the umbrella view and per-product reference. Deep,
  code-adjacent docs continue to live in each repository — the hub **links** to them.

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
| [Alephee](partners/alephee/) | Marketplace integration platform (engineering partner) | [reference](partners/alephee/reference/) |
| [Noordhen](partners/noordhen/) | Custom operations platform for Noordhen Brasil (support partner) | [reference](partners/noordhen/reference/) |

### 🏭 [OGS Studio](studio/) — *scalable, packaged*
| Product | What it is | Docs |
|---|---|---|
| [Press](studio/press/) | Content-site platform — OSS (self-host) and Cloud (agencies) | [reference](studio/press/reference/) |
| [Co.](studio/co/) | Done-for-you IT services for SMBs | [explanation](studio/co/explanation/) |
| [Royale IQ](studio/royale-iq/) | AI coach for Clash Royale players (pro bono) | [reference](studio/royale-iq/reference/) |

### ⚙️ [OGS Engine](engine/) — *the machine room*
| Engine | What it is | Docs |
|---|---|---|
| [Press](engine/press/) | CMS core (`@nis/create` scaffolder) | [reference](engine/press/reference/) |
| [Agent AI](engine/agent-ai/) | AI core powering Royale IQ | [reference](engine/agent-ai/reference/) |
| [Superset AI](engine/superset-ai/) | Internal Claude-tooling desktop apps | [reference](engine/superset-ai/reference/) |

---

## Understanding the framework

Each product folder uses the four Diátaxis quadrants:

| Quadrant | Orientation | Answers |
|---|---|---|
| 📚 **Tutorials** | learning | "Teach me, step by step" |
| 🔧 **How-to guides** | tasks | "How do I accomplish X?" |
| 📖 **Reference** | information | "What is the exact API / command / config?" |
| 💡 **Explanation** | understanding | "Why is it built this way?" |

> In this first pass, **Reference** and **Explanation** are written from the real
> repositories; **Tutorials** and **How-to** are guided stubs ready to be filled.

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
  the *technical* reference; Studio holds the *product / go-to-market* framing and cross-links.
- **Link, don't duplicate:** if a repo already has good docs, link to them from `reference/`.
- **Markdown only:** no build step, no dependencies (see [CLAUDE.md](../CLAUDE.md)).

---

*Odenir Gomes Solutions (OGS) · CNPJ 54.705.657/0001-83 · São Paulo/SP · founded 2024-04-12*
*[ogsolucoes.com.br](https://ogsolucoes.com.br)*
