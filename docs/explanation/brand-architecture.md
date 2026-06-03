# Brand Architecture — the OGS umbrella

> *Understanding-oriented.* This page explains how OGS Tech is structured as a **brand
> umbrella**, why each brand exists, and where every product and service fits.

OGS Tech (legal entity **Odenir Gomes Solutions**, CNPJ 54.705.657/0001-83, São Paulo/SP)
operates three brands under one umbrella. Each brand is a different **way of going to market**
with the same underlying technology.

```
                          OGS Tech · Brazil
                     "Your business. Further." · Future Ready
                                  │
        ┌─────────────────────────┼─────────────────────────┐
        │                         │                          │
   OGS Partners              OGS Studio                  OGS Engine
   premium                   scalable                    machine room
   useogs.com/partners       useogs.com/studio           (internal)
```

---

## OGS Partners — *premium, bespoke, high-margin*

**Services OGS provides** to partner companies, **executed by OGS Engine** — and deliverables
**may use the Press**. Two service types:

| Service | What OGS provides | Partner |
|---|---|---|
| **Engineering** | Software engineering as a service | **Alephee** — building its marketplace integration platform |
| **Support** | Ongoing operations support | **Noordhen** — custom operations platform for Noordhen Brasil |

→ Docs: [partners/](../partners/)

---

## OGS Studio — *scalable, packages & sells*

Studio takes what Engine builds, **packages it as a product, and sells it**. It has three offers:

### Press — three doors, one engine
The Press (CMS core, built by Engine) is sold through three doors depending on the buyer:

| Door | Audience | Model |
|---|---|---|
| **Open Source** | developers | free, self-hosted |
| **Cloud** | agencies | managed, paid |
| **Co.** | SMBs | done-for-you (Studio Co. runs the Press for them) |

### Co. — *done-for-you IT services*
OGS Studio Co. provides managed IT services and **operates the Press** on behalf of clients.

| Segment | Audience | Note |
|---|---|---|
| **Empresas** *(primary)* | Brazilian SMBs | the main revenue segment |
| **Influencers** *(niche)* | creators treated as a company | includes **Royale IQ** |

### Royale IQ — *pro bono, influencers niche*
An AI coach for Clash Royale players. Powered by **Agent AI** (Engine). Positioned as pro bono
within the influencers niche.

→ Docs: [studio/](../studio/)

---

## OGS Engine — *the machine room*

Engine builds the technology and executes Partners' projects. It is where the **product engines**
live. Two engines graduate into products; one is an internal tool.

| Component | Type | Becomes |
|---|---|---|
| **Press** | product engine · CMS core | → OGS Studio Press |
| **Agent AI** | product engine · AI core | → the Royale IQ app |
| **Superset AI** | internal tool | desktop app that helps the team use Claude and its adaptations |

→ Docs: [engine/](../engine/)

---

## Mapping brands to repositories

The brand umbrella does not map 1:1 to folders on disk. This is the canonical mapping:

| Brand path | Repository / folder |
|---|---|
| Partners · Engineering | `alephee/` (+ 6 sub-services) |
| Partners · Support | `noordhen/` |
| Studio · Press (OSS) / Engine · Press | `internal/cloud-press-cli` (Cloud Press CLI) |
| Studio · Press (Cloud) | `internal/cloud-press-cloud` |
| Studio · Royale IQ / Engine · Agent AI | `internal/royale-agent-ai-app` |
| Engine · Superset AI | `internal/sde-superset-ai-app` (SDE Superset AI App) + `internal/company-superset-ai-app` (Company Superset AI App) |

> **Why Engine vs Studio for the same repo?** A single codebase can appear under both brands.
> Engine documents *how it is built* (technical reference); Studio documents *how it is packaged
> and sold* (product framing). The two cross-link rather than duplicate.

Legacy and archived projects (`_legacy/`) are intentionally **not** documented here.

---

See also: [How it connects](how-it-connects.md) · [Glossary](glossary.md)
